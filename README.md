## The Repositiories

Different architectonical elements of the Pick By Light project are stored in different repositories.
So to help you find what you need, here is a list of repos with their contents.

### [Backend](https://github.com/PBL-Pick-By-Light/BE-Backend)

The [backend repo](https://github.com/PBL-Pick-By-Light/BE-Backend) contains code for a server with
- authorization
- database
- controllers
- http-Tests
- docker
  You can also start by reading the [documentation](https://git.thm.de/softwaretechnik-projekt-pick-by-light-system-wise21_22/pbl-backend/pbl-backend/-/wikis/home).

### [Frontend](https://github.com/PBL-Pick-By-Light/FE-Frontend)

The graphical user interface allows the user to interact with the system and sends requests to the backend and embedded system. A login system ensures that only authorized users can use the system. The desired parts are selected via a search mask and displayed via the further connection. Extended setting options are available to the administrator. Parts and shelfs can be created and managed.

From a technical point of view, the frontend is realized with vue and vuetify and is running in a nginx docker container. The different components are presented on individual pages.

### Embedded Systems

Everything you need to physically build the project and code for low-level servers.

#### [Hardware Design](https://github.com/PBL-Pick-By-Light/ES-hardware-design)
Files for 3D-printing and explainations on how to upgrade your shelves using LEDs.

#### [HTTP to MQTT](https://github.com/PBL-Pick-By-Light/ES-HttpToMqtt)
Code for a server that translates HTTP-Requests and sends corresponding MQTT messages to the ESP32s.

#### [Firmware](https://github.com/PBL-Pick-By-Light/ES-ESP32-firmware)
Firmware of the ESP32s, which receive the MQTT messages and control the LEDs.

#### [ES Documentation](https://github.com/PBL-Pick-By-Light/ES-Wiki-and-Documentation)
Further infos on the embedded systems part of the project.

## Contributing

If you are new to the project, we recommend reading the docs of the respective repository (as listed above).

**You want to make a contribution to the project?**

[Here](https://github.com/PBL-Pick-By-Light/Pick_By_Light/issues) you can find a list of Issues you can work on.
Also check the Issues in the Sub-Repositiories.
New features and code changes are organized throug Pull Requests.
If you're new to the concept, check out [this](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests) description.

**You have discovered a bug or have an idea for a new feature?**

You can add a new Issue [here](https://github.com/PBL-Pick-By-Light/Pick_By_Light/issues).


**When changes are made, check if other repositories are affected!**

Example:
In the backend repo, the attribute `name` in User entity is changed to `username`.
Because this affects the frontend, one should check the frontend repo before commiting the changes.

**Build instructions** can be found in the README files of the repos.

## Licensing

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License.

You may obtain a copy of the License from [here](https://github.com/PBL-Pick-By-Light/Pick_By_Light/blob/main/LICENSE).

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the LICENSE for the specific language governing permissions and limitations under the License.
