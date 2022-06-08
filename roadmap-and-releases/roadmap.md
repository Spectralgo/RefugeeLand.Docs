# Roadmap

## Refugee.Core Api 0.1.0

### 🎯 Refugee has RefugeeGroup

* [ ] INFRA
  * [x] INFRA: Initialize API Project
  * [x] INFRA: Initialize Build Pipelines
  * [x] INFRA: Initialize Unit Tests Project
  * [x] INFRA: Initialize Refugee Core Provision
  * [ ] INFRA: Initialize Release Project
  * [ ] INFRA: Initialize Acceptance Test Project
* [ ] DATA
  * [x] DATA: Add Refugee Model & Migrations
    * [x] Nationalities
    * [x] MedicalConditions
    * [ ] Pets
    * [x] Languages
  * [x] DATA: Add RefugeeGroup Model & Migrations
  * [x] DATA: Enums
    * [x] Fluency Level
    * [ ] PetType
    * [x] Gender
* [ ] CONTROLLERS
  * [x] CONTROLLERS: POST Refugee
  * [ ] CONTROLLERS: GET All Refugees
  * [ ] CONTROLLERS: GET Specific Refugee by Id
  * [ ] CONTROLLERS: PUT Refugee
  * [ ] CONTROLLERS: DELETE Refugee
  * [ ] CONTROLLERS: POST RefugeeGroup
  * [ ] CONTROLLERS: GET All RefugeeGroups
  * [ ] CONTROLLERS: GET Specific RefugeeGroup
  * [ ] CONTROLLERS: PUT RefugeeGroup
  * [ ] CONTROLLERS: DELETE RefugeeGroup
* [ ] FOUNDATION SERVICES
  * [x] FOUNDATIONS: Add Refugee
  * [ ] FOUNDATIONS: Retrieve All Refugees
  * [ ] FOUNDATIONS: Retrieve Specific Refugee by Id
  * [ ] FOUNDATIONS: Modify Refugee
  * [ ] FOUNDATIONS: Remove Refugee
  * [ ] FOUNDATIONS: Add RefugeeGroup
  * [ ] FOUNDATIONS: Retrieve All RefugeeGroups
  * [ ] FOUNDATIONS: Retrieve Specific RefugeeGroup
  * [ ] FOUNDATIONS: Modify RefugeeGroup
  * [ ] FOUNDATIONS: Remove RefugeeGroup
* [ ] BROKERS
  * [x] BROKERS: Setup Storage Broker
  * [x] BROKERS: Insert Refugee
  * [x] BROKERS: Select All Refugees
  * [x] BROKERS: Select Specific Refugee by Id
  * [x] BROKERS: Update Refugee
  * [x] BROKERS: Delete Refugee
  * [ ] BROKERS: Insert RefugeeGroup
  * [ ] BROKERS: Select All RefugeeGroups
  * [ ] BROKERS: Select Specific RefugeeGroup by Id
  * [ ] BROKERS: Update RefugeeGroup
  * [ ] BROKERS: Delete RefugeeGroup

### 🎯 Host has Shelters

* [ ] DATA
  * [ ] DATA: Add Host Model & Migrations
    * [ ] Contatinformation
    * [ ] Shelters
  * [ ] DATA: Add Shelter Model & Migrations
    * [ ] Pets
  * [ ] DATA: Enums
    * [ ] PetType renaming
* [ ] CONTROLLERS
  * [ ] CONTROLLER: POST Host
  * [ ] CONTROLLER: GET All Hosts
  * [ ] CONTROLLER: GET Specific Host by Id
  * [ ] CONTROLLER: PUT Host
  * [ ] CONTROLLER: DELETE Host
  * [ ] CONTROLLER: POST Shelter
  * [ ] CONTROLLER: GET All Shelter
  * [ ] CONTROLLER: GET Specific Shelter by Id
  * [ ] CONTROLLER: PUT Shelter
  * [ ] CONTROLLER: DELETE Shelter
* [ ] FOUNDATION SERVICES
  * [ ] FOUNDATIONS: Add Host
  * [ ] FOUNDATIONS: Retrieve All Hosts
  * [ ] FOUNDATIONS: Retrieve Specific Host by Id
  * [ ] FOUNDATIONS: Modify Host
  * [ ] FOUNDATIONS: Remove Host
  * [ ] FOUNDATIONS: Add Shelter
  * [ ] FOUNDATIONS: Retrieve All Shelters
  * [ ] FOUNDATIONS: Retrieve Specific Shelter
  * [ ] FOUNDATIONS: Modify Shelter
  * [ ] FOUNDATIONS: Remove Shelter
* [ ] BROKERS
  * [ ] BROKERS: Setup Storage Broker
  * [ ] BROKERS: Insert Host
  * [ ] BROKERS: Select All Hosts
  * [ ] BROKERS: Select Specific Host by Id
  * [ ] BROKERS: Update Host
  * [ ] BROKERS: Delete Host
  * [ ] BROKERS: Insert Shelter
  * [ ] BROKERS: Select All Shelters
  * [ ] BROKERS: Select Specific Shelter by Id
  * [ ] BROKERS: Update Shelter
  * [ ] BROKERS: Delete Shelter

### 🎯 Host create ShelterOffer

### 🎯 Refugee can look at ShelterOffers

### 🎯 Refugee sends a ShelterRequest for a particular ShelterOffer

### 🎯 Host sees ShelterRequests

### 🎯 Host accept or reject ShelterRequest

## Refugee.Core Api 0.2.0

wip
