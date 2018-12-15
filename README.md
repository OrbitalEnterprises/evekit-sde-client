# EveKit SDE auto-generated client

This client is auto-generated by the Swagger codegen maven plugin.

The auto-generated instructions in the installation are appended below but are not quite correct.  Please use the following instructions instead.

## Using the Library

A regular release of this library is deposited in [Maven Central](https://search.maven.org/).  Releases of the library are versioned by build date of the form `YYYYMMDD`.

For maven, add this dependency to your project's POM (substitute YYYYMMDD as appropriate):

```xml
<dependency>
    <groupId>enterprises.orbital.evekit</groupId>
    <artifactId>sde.client</artifactId>
    <version>1.0.0.YYYYMMDD</version>
    <scope>compile</scope>
</dependency>
```

For gradle, add this dependency to your project's build file (substitute YYYYMMDD as appropriate):

```groovy
compile "enterprises.orbital.evekit:sde.client:1.0.0.YYYYMMDD"
```

For everyone else, you'll need to first build the library with Maven as described below, then manually install the following JARs in the appropriate places (substitute YYYYMMDD as appropriate):

* target/evekit-sde-client-1.0.0.YYYYMMDD.jar
* target/lib/*.jar

## Building the Library

The library should build cleanly out of the box with Maven as follows (we assume Java 1.8):

    mvn clean package

The `package` build phase includes a final assembly script which moves documentation to the correct location and builds this README file.

The library is always built based on the latest online Swagger specification for the EVE Swagger Interface.  You can build off of a downloaded specification instead by changing the `inputSpec` property of the `generate` goal in the POM file.

# Auto-Generated Installation Instructions

# swagger-java-client

## Requirements

Building the API client library requires [Maven](https://maven.apache.org/) to be installed.

## Installation

To install the API client library to your local Maven repository, simply execute:

```shell
mvn install
```

To deploy it to a remote Maven repository instead, configure the settings of the repository and execute:

```shell
mvn deploy
```

Refer to the [official documentation](https://maven.apache.org/plugins/maven-deploy-plugin/usage.html) for more information.

### Maven users

Add this dependency to your project's POM:

```xml
<dependency>
    <groupId>io.swagger</groupId>
    <artifactId>swagger-java-client</artifactId>
    <version>1.0.0</version>
    <scope>compile</scope>
</dependency>
```

### Gradle users

Add this dependency to your project's build file:

```groovy
compile "io.swagger:swagger-java-client:1.0.0"
```

### Others

At first generate the JAR by executing:

    mvn package

Then manually install the following JARs:

* target/swagger-java-client-1.0.0.jar
* target/lib/*.jar

## Getting Started

Please follow the [installation](#installation) instruction and execute the following Java code:

```java

import enterprises.orbital.evekit.sde.client.invoker.*;
import enterprises.orbital.evekit.sde.client.invoker.auth.*;
import enterprises.orbital.evekit.sde.client.model.*;
import enterprises.orbital.evekit.sde.client.api.AgentApi;

import java.io.File;
import java.util.*;

public class AgentApiExample {

    public static void main(String[] args) {
        
        AgentApi apiInstance = new AgentApi();
        Integer contid = -1; // Integer | Continuation ID for paged results
        Integer maxresults = 1000; // Integer | Maximum number of results to retrieve
        String agentTypeID = "{ any: true }"; // String | Agent type ID selector
        String agentType = "{ any: true }"; // String | Agent type name selector
        try {
            List<AgtAgentType> result = apiInstance.getAgentTypes(contid, maxresults, agentTypeID, agentType);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling AgentApi#getAgentTypes");
            e.printStackTrace();
        }
    }
}

```

## Documentation for API Endpoints

All URIs are relative to *https://evekit-sde.orbital.enterprises/20181214/api/ws/v20181214*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AgentApi* | [**getAgentTypes**](docs/AgentApi.md#getAgentTypes) | **GET** /agt/agentType | Get agent types
*AgentApi* | [**getAgents**](docs/AgentApi.md#getAgents) | **GET** /agt/agent | Get agents
*AgentApi* | [**getResearchAgents**](docs/AgentApi.md#getResearchAgents) | **GET** /agt/researchAgent | Get research agents
*CertificatesApi* | [**getCertificateMasteries**](docs/CertificatesApi.md#getCertificateMasteries) | **GET** /crt/mastery | Get certificate masteries
*CertificatesApi* | [**getCertificateSkills**](docs/CertificatesApi.md#getCertificateSkills) | **GET** /crt/skill | Get certificate skills
*CertificatesApi* | [**getCertificates**](docs/CertificatesApi.md#getCertificates) | **GET** /crt/certificate | Get certificates
*CharacterApi* | [**getAncestries**](docs/CharacterApi.md#getAncestries) | **GET** /chr/ancestry | Get ancestries
*CharacterApi* | [**getAttributes**](docs/CharacterApi.md#getAttributes) | **GET** /chr/attribute | Get attributes
*CharacterApi* | [**getBloodlines**](docs/CharacterApi.md#getBloodlines) | **GET** /chr/bloodline | Get bloodlines
*CharacterApi* | [**getFactions**](docs/CharacterApi.md#getFactions) | **GET** /chr/faction | Get factions
*CharacterApi* | [**getRaces**](docs/CharacterApi.md#getRaces) | **GET** /chr/race | Get races
*CorporationApi* | [**getCorpActivities**](docs/CorporationApi.md#getCorpActivities) | **GET** /crp/activity | Get corporation activities
*CorporationApi* | [**getNpcCorporationDivisions**](docs/CorporationApi.md#getNpcCorporationDivisions) | **GET** /crp/npc_corp_division | Get NPC corporation divisions
*CorporationApi* | [**getNpcCorporationResearchFields**](docs/CorporationApi.md#getNpcCorporationResearchFields) | **GET** /crp/npc_corp_research_field | Get NPC corporation research fields
*CorporationApi* | [**getNpcCorporationTrades**](docs/CorporationApi.md#getNpcCorporationTrades) | **GET** /crp/npc_corp_trade | Get NPC corporation trades
*CorporationApi* | [**getNpcCorporations**](docs/CorporationApi.md#getNpcCorporations) | **GET** /crp/npc_corp | Get NPC corporations
*CorporationApi* | [**getNpcDivisions**](docs/CorporationApi.md#getNpcDivisions) | **GET** /crp/npc_division | Get NPC divisions
*DogmaApi* | [**getAttributeCategories**](docs/DogmaApi.md#getAttributeCategories) | **GET** /dgm/attribute_category | Get attribute categories
*DogmaApi* | [**getAttributeTypes**](docs/DogmaApi.md#getAttributeTypes) | **GET** /dgm/attribute_type | Get attribute types
*DogmaApi* | [**getEffects**](docs/DogmaApi.md#getEffects) | **GET** /dgm/effect | Get effects
*DogmaApi* | [**getExpressions**](docs/DogmaApi.md#getExpressions) | **GET** /dgm/expression | Get expressions
*DogmaApi* | [**getTypeAttributes**](docs/DogmaApi.md#getTypeAttributes) | **GET** /dgm/type_attribute | Get type attributes
*DogmaApi* | [**getTypeEffects**](docs/DogmaApi.md#getTypeEffects) | **GET** /dgm/type_effect | Get type effects
*EVEApi* | [**getGraphics**](docs/EVEApi.md#getGraphics) | **GET** /eve/graphic | Get graphics
*EVEApi* | [**getIcons**](docs/EVEApi.md#getIcons) | **GET** /eve/icon | Get icons
*EVEApi* | [**getUnits**](docs/EVEApi.md#getUnits) | **GET** /eve/unit | Get units
*IndustryApi* | [**getActivities**](docs/IndustryApi.md#getActivities) | **GET** /ind/activity | Get industry activities
*IndustryApi* | [**getActivityMaterials**](docs/IndustryApi.md#getActivityMaterials) | **GET** /ind/activity_material | Get industry activity materials
*IndustryApi* | [**getActivityProbabilities**](docs/IndustryApi.md#getActivityProbabilities) | **GET** /ind/activity_probability | Get industry activity probabilities
*IndustryApi* | [**getActivityProducts**](docs/IndustryApi.md#getActivityProducts) | **GET** /ind/activity_product | Get industry activity products
*IndustryApi* | [**getActivitySkills**](docs/IndustryApi.md#getActivitySkills) | **GET** /ind/activity_skill | Get industry activity skills
*IndustryApi* | [**getBlueprintTypes**](docs/IndustryApi.md#getBlueprintTypes) | **GET** /ind/blueprint | Get blueprints
*InventoryApi* | [**getCategories**](docs/InventoryApi.md#getCategories) | **GET** /inv/category | Get categories
*InventoryApi* | [**getContrabandTypes**](docs/InventoryApi.md#getContrabandTypes) | **GET** /inv/contraband_type | Get contraband types
*InventoryApi* | [**getControlTowerResourcePurposes**](docs/InventoryApi.md#getControlTowerResourcePurposes) | **GET** /inv/control_tower_resource_purpose | Get control tower resource purposes
*InventoryApi* | [**getControlTowerResources**](docs/InventoryApi.md#getControlTowerResources) | **GET** /inv/control_tower_resource | Get control tower resources
*InventoryApi* | [**getFlags**](docs/InventoryApi.md#getFlags) | **GET** /inv/flag | Get flags
*InventoryApi* | [**getGroups**](docs/InventoryApi.md#getGroups) | **GET** /inv/group | Get groups
*InventoryApi* | [**getItems**](docs/InventoryApi.md#getItems) | **GET** /inv/item | Get items
*InventoryApi* | [**getMetaGroups**](docs/InventoryApi.md#getMetaGroups) | **GET** /inv/meta_group | Get meta groups
*InventoryApi* | [**getMetaTypes**](docs/InventoryApi.md#getMetaTypes) | **GET** /inv/meta_type | Get meta types
*InventoryApi* | [**getNames**](docs/InventoryApi.md#getNames) | **GET** /inv/name | Get names
*InventoryApi* | [**getPositions**](docs/InventoryApi.md#getPositions) | **GET** /inv/position | Get positions
*InventoryApi* | [**getTraits**](docs/InventoryApi.md#getTraits) | **GET** /inv/trait | Get traits
*InventoryApi* | [**getTypeMaterials**](docs/InventoryApi.md#getTypeMaterials) | **GET** /inv/type_material | Get type materials
*InventoryApi* | [**getTypeReactions**](docs/InventoryApi.md#getTypeReactions) | **GET** /inv/type_reaction | Get type reactions
*InventoryApi* | [**getTypes**](docs/InventoryApi.md#getTypes) | **GET** /inv/type | Get types
*InventoryApi* | [**getUniqueNames**](docs/InventoryApi.md#getUniqueNames) | **GET** /inv/unique_name | Get unique names
*InventoryApi* | [**getVolumes**](docs/InventoryApi.md#getVolumes) | **GET** /inv/volume | Get type volumes
*MapApi* | [**getCelestialStatistics**](docs/MapApi.md#getCelestialStatistics) | **GET** /map/celestial_statistic | Get celestial statistics
*MapApi* | [**getConstellationJumps**](docs/MapApi.md#getConstellationJumps) | **GET** /map/constellation_jump | Get constellation jumps
*MapApi* | [**getConstellations**](docs/MapApi.md#getConstellations) | **GET** /map/constellation | Get constellations
*MapApi* | [**getDenormalization**](docs/MapApi.md#getDenormalization) | **GET** /map/denormalize | Get denormalization
*MapApi* | [**getJumps**](docs/MapApi.md#getJumps) | **GET** /map/jump | Get jumps
*MapApi* | [**getLocationScenes**](docs/MapApi.md#getLocationScenes) | **GET** /map/location_scene | Get location scenes
*MapApi* | [**getLocationWormholeClasses**](docs/MapApi.md#getLocationWormholeClasses) | **GET** /map/location_wormhole_class | Get location wormhole classes
*MapApi* | [**getRegionJumps**](docs/MapApi.md#getRegionJumps) | **GET** /map/region_jump | Get region jumps
*MapApi* | [**getRegions**](docs/MapApi.md#getRegions) | **GET** /map/region | Get regions
*MapApi* | [**getSolarSystemJumps**](docs/MapApi.md#getSolarSystemJumps) | **GET** /map/solar_system_jump | Get solar system jumps
*MapApi* | [**getSolarSystems**](docs/MapApi.md#getSolarSystems) | **GET** /map/solar_system | Get solar systems
*MapApi* | [**getUniverses**](docs/MapApi.md#getUniverses) | **GET** /map/universe | Get universes
*PlanetApi* | [**getSchematicPinMaps**](docs/PlanetApi.md#getSchematicPinMaps) | **GET** /plt/schematic_pin_map | Get schematic pin maps
*PlanetApi* | [**getSchematicTypeMaps**](docs/PlanetApi.md#getSchematicTypeMaps) | **GET** /plt/schematic_type_map | Get schematic type maps
*PlanetApi* | [**getSchematics**](docs/PlanetApi.md#getSchematics) | **GET** /plt/schematic | Get schematics
*RAMApi* | [**getAssemblyLineStations**](docs/RAMApi.md#getAssemblyLineStations) | **GET** /ram/assembly_line_station | Get assembly line stations
*RAMApi* | [**getAssemblyLineTypeDetailsPerCategory**](docs/RAMApi.md#getAssemblyLineTypeDetailsPerCategory) | **GET** /ram/assembly_line_type_detail_per_category | Get assembly line type details per category
*RAMApi* | [**getAssemblyLineTypeDetailsPerGroup**](docs/RAMApi.md#getAssemblyLineTypeDetailsPerGroup) | **GET** /ram/assembly_line_type_detail_per_group | Get assembly line type details per group
*RAMApi* | [**getAssemblyLineTypes**](docs/RAMApi.md#getAssemblyLineTypes) | **GET** /ram/assembly_line_type | Get assembly line types
*RAMApi* | [**getInstallationTypeContents**](docs/RAMApi.md#getInstallationTypeContents) | **GET** /ram/installation_type_content | Get installation type contents
*RAMApi* | [**getRAMActivities**](docs/RAMApi.md#getRAMActivities) | **GET** /ram/activity | Get activities
*SkinApi* | [**getLicenses**](docs/SkinApi.md#getLicenses) | **GET** /skn/license | Get licenses
*SkinApi* | [**getMaterials**](docs/SkinApi.md#getMaterials) | **GET** /skn/material | Get materials
*SkinApi* | [**getShips**](docs/SkinApi.md#getShips) | **GET** /skn/ship | Get ships
*SkinApi* | [**getSkins**](docs/SkinApi.md#getSkins) | **GET** /skn/skin | Get skins
*StationApi* | [**getOperationServices**](docs/StationApi.md#getOperationServices) | **GET** /sta/operation_service | Get operation services
*StationApi* | [**getOperations**](docs/StationApi.md#getOperations) | **GET** /sta/operation | Get operations
*StationApi* | [**getServices**](docs/StationApi.md#getServices) | **GET** /sta/service | Get services
*StationApi* | [**getStationTypes**](docs/StationApi.md#getStationTypes) | **GET** /sta/station_type | Get station types
*StationApi* | [**getStations**](docs/StationApi.md#getStations) | **GET** /sta/station | Get stations
*TranslationApi* | [**getColumns**](docs/TranslationApi.md#getColumns) | **GET** /trn/column | Get columns
*TranslationApi* | [**getLanguages**](docs/TranslationApi.md#getLanguages) | **GET** /trn/language | Get languages
*TranslationApi* | [**getTranslations**](docs/TranslationApi.md#getTranslations) | **GET** /trn/translation | Get translations
*WarApi* | [**getCombatZoneSystems**](docs/WarApi.md#getCombatZoneSystems) | **GET** /war/combat_zone_system | Get combat zone systems
*WarApi* | [**getCombatZones**](docs/WarApi.md#getCombatZones) | **GET** /war/combat_zone | Get combat zones


## Documentation for Models

 - [AgtAgent](docs/AgtAgent.md)
 - [AgtAgentType](docs/AgtAgentType.md)
 - [AgtResearchAgent](docs/AgtResearchAgent.md)
 - [ChrAncestry](docs/ChrAncestry.md)
 - [ChrAttribute](docs/ChrAttribute.md)
 - [ChrBloodline](docs/ChrBloodline.md)
 - [ChrFaction](docs/ChrFaction.md)
 - [ChrRace](docs/ChrRace.md)
 - [CrpActivity](docs/CrpActivity.md)
 - [CrpNpcCorporation](docs/CrpNpcCorporation.md)
 - [CrpNpcCorporationDivision](docs/CrpNpcCorporationDivision.md)
 - [CrpNpcCorporationResearchField](docs/CrpNpcCorporationResearchField.md)
 - [CrpNpcCorporationTrade](docs/CrpNpcCorporationTrade.md)
 - [CrpNpcDivision](docs/CrpNpcDivision.md)
 - [CrtCertificate](docs/CrtCertificate.md)
 - [CrtMastery](docs/CrtMastery.md)
 - [CrtSkill](docs/CrtSkill.md)
 - [DgmAttributeCategory](docs/DgmAttributeCategory.md)
 - [DgmAttributeType](docs/DgmAttributeType.md)
 - [DgmEffect](docs/DgmEffect.md)
 - [DgmExpression](docs/DgmExpression.md)
 - [DgmTypeAttribute](docs/DgmTypeAttribute.md)
 - [DgmTypeEffect](docs/DgmTypeEffect.md)
 - [EveGraphic](docs/EveGraphic.md)
 - [EveIcon](docs/EveIcon.md)
 - [EveUnit](docs/EveUnit.md)
 - [IndActivity](docs/IndActivity.md)
 - [IndActivityMaterial](docs/IndActivityMaterial.md)
 - [IndActivityProbability](docs/IndActivityProbability.md)
 - [IndActivityProduct](docs/IndActivityProduct.md)
 - [IndActivitySkill](docs/IndActivitySkill.md)
 - [IndBlueprint](docs/IndBlueprint.md)
 - [InvCategory](docs/InvCategory.md)
 - [InvContrabandType](docs/InvContrabandType.md)
 - [InvControlTowerResource](docs/InvControlTowerResource.md)
 - [InvControlTowerResourcePurpose](docs/InvControlTowerResourcePurpose.md)
 - [InvFlag](docs/InvFlag.md)
 - [InvGroup](docs/InvGroup.md)
 - [InvItem](docs/InvItem.md)
 - [InvMetaGroup](docs/InvMetaGroup.md)
 - [InvMetaType](docs/InvMetaType.md)
 - [InvName](docs/InvName.md)
 - [InvPosition](docs/InvPosition.md)
 - [InvTrait](docs/InvTrait.md)
 - [InvType](docs/InvType.md)
 - [InvTypeMaterial](docs/InvTypeMaterial.md)
 - [InvTypeReaction](docs/InvTypeReaction.md)
 - [InvUniqueName](docs/InvUniqueName.md)
 - [InvVolume](docs/InvVolume.md)
 - [MapCelestialStatistic](docs/MapCelestialStatistic.md)
 - [MapConstellation](docs/MapConstellation.md)
 - [MapConstellationJump](docs/MapConstellationJump.md)
 - [MapDenormalize](docs/MapDenormalize.md)
 - [MapJump](docs/MapJump.md)
 - [MapLocationScene](docs/MapLocationScene.md)
 - [MapLocationWormholeClass](docs/MapLocationWormholeClass.md)
 - [MapRegion](docs/MapRegion.md)
 - [MapRegionJump](docs/MapRegionJump.md)
 - [MapSolarSystem](docs/MapSolarSystem.md)
 - [MapSolarSystemJump](docs/MapSolarSystemJump.md)
 - [MapUniverse](docs/MapUniverse.md)
 - [PltSchematic](docs/PltSchematic.md)
 - [PltSchematicsPinMap](docs/PltSchematicsPinMap.md)
 - [PltSchematicsTypeMap](docs/PltSchematicsTypeMap.md)
 - [RamActivity](docs/RamActivity.md)
 - [RamAssemblyLineStation](docs/RamAssemblyLineStation.md)
 - [RamAssemblyLineType](docs/RamAssemblyLineType.md)
 - [RamAssemblyLineTypeDetailPerCategory](docs/RamAssemblyLineTypeDetailPerCategory.md)
 - [RamAssemblyLineTypeDetailPerGroup](docs/RamAssemblyLineTypeDetailPerGroup.md)
 - [RamInstallationTypeContent](docs/RamInstallationTypeContent.md)
 - [ServiceError](docs/ServiceError.md)
 - [SknLicense](docs/SknLicense.md)
 - [SknMaterial](docs/SknMaterial.md)
 - [SknShip](docs/SknShip.md)
 - [SknSkin](docs/SknSkin.md)
 - [StaOperation](docs/StaOperation.md)
 - [StaOperationService](docs/StaOperationService.md)
 - [StaService](docs/StaService.md)
 - [StaStation](docs/StaStation.md)
 - [StaStationType](docs/StaStationType.md)
 - [TrnTranslation](docs/TrnTranslation.md)
 - [TrnTranslationColumn](docs/TrnTranslationColumn.md)
 - [TrnTranslationLanguage](docs/TrnTranslationLanguage.md)
 - [WarCombatZone](docs/WarCombatZone.md)
 - [WarCombatZoneSystem](docs/WarCombatZoneSystem.md)


## Documentation for Authorization

All endpoints do not require authorization.
Authentication schemes defined for the API:

## Recommendation

It's recommended to create an instance of `ApiClient` per thread in a multithreaded environment to avoid any potential issues.

## Author



