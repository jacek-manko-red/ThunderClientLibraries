# If not stated otherwise in this file or this component's LICENSE file the
# following copyright and licenses apply:
#
# Copyright 2020 Metrological
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

option(BLUETOOTHAUDIOSINK
        "Include the bluetoothaudiosink library." OFF)
option(PROTOCOLS
        "Include the protocols library." ON)
option(COMPOSITORCLIENT
        "Include a graphics backend abstraction for external applications." OFF)
option(GSTREAMERCLIENT
        "Include a gstreamer sink abstraction for external applications." OFF)
option(DEVICEINFO
        "Include the deviceinfo COMRPC abstraction library." OFF)
option(DISPLAYINFO
        "Include the displayinfo COMRPC abstraction library." OFF)
option(SECURITYAGENT
        "Include the securityagent library." OFF)
option(PLAYERINFO
        "Include the playerinfo COMRPC abstraction library." OFF)
option(PROVISIONPROXY
        "Include the provisionproxy library." OFF)
option(CDMI
        "Include OpenCDM interface." OFF)
option(CRYPTOGRAPHY
        "Include the cryptography library." OFF)
option(LOCALTRACER
        "Header only library to locally print traces coming from Messaging without the need of running Thunder/WPEFramework." OFF)

if(BLUETOOTHAUDIOSINK)
    add_subdirectory(bluetoothaudiosink)
endif()

if(COMPOSITORCLIENT)
    add_subdirectory(compositorclient)
endif()

if(GSTREAMERCLIENT)
    add_subdirectory(gstreamerclient)
endif()

if(DEVICEINFO)
    add_subdirectory(deviceinfo)
endif()

if(DISPLAYINFO)
    add_subdirectory(displayinfo)
endif()

if(SECURITYAGENT)
    add_subdirectory(securityagent)
endif()

if(PLAYERINFO)
    add_subdirectory(playerinfo)
endif()

if(PROVISIONPROXY)
    add_subdirectory(provisionproxy)
endif()

if(VIRTUALINPUT)
    add_subdirectory(virtualinput)
endif()

if(CDMI)
    add_subdirectory(ocdm)
endif()

if(CRYPTOGRAPHY)
    add_subdirectory(cryptography)
endif()

if(LOCALTRACER)
    add_subdirectory(localtracer)
endif()
