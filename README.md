# dairyFirmOntology

## Dairy Firm Ontology - Knowledge Representation

The ontology is organized into the following main classes, each with multiple levels of subclasses to capture the detailed aspects of human rights:



  DairyFirm
1.  Livestock 
   -  Cow 
     - DairyCow
       - JerseyCow
       - HolsteinCow
       - AyrshireCow
     - BeefCow
       - AngusCow
       - HerefordCow
       - CharolaisCow
     - PregnantCow
       - FirstTrimester
       - SecondTrimester
       - ThirdTrimester
   -  Buffalo 
     - DairyBuffalo
       - MurrahBuffalo
       - JaffarabadiBuffalo
       - SurtiBuffalo
     - RiverBuffalo
       - ChineseRiverBuffalo
       - IndianRiverBuffalo
       - ThaiRiverBuffalo
   -  Goat 
     - DairyGoat
       - SaanenGoat
       - NubianGoat
       - ToggenburgGoat
     - MeatGoat
       - BoerGoat
       - KikoGoat
       - SpanishGoat

2.  MilkingProcess 
   - MilkingMachine
     - AutomatedMilkingSystem
       - RoboticMilkingArm
       - SensorBasedMilking
     - RotaryMilkingParlor
       - ParallelParlor
       - TandemParlor
   - HandMilking
     - TraditionalHandMilking
       - OpenHandMilking
       - ControlledHandMilking
       - EmergencyHandMilking

3.  FeedingSystem 
   - FodderManagement
     - FreshFodder
       - GrassFodder
       - GreenLegumeFodder
       - HydroponicFodder
       - SeasonalFodder
     - DriedFodder
       - AlfalfaHay
       - StrawHay
       - GrassHay
   - SupplementaryFeeding
     - MineralSupplements
       - CalciumSupplements
       - PhosphorusSupplements
       - MagnesiumSupplements
       - SaltSupplements
     - VitaminSupplements
       - VitaminA
       - VitaminB
       - VitaminC
       - VitaminD

4.  AnimalHealth 
   - VeterinaryCheckup
     - RoutineCheckup
       - MonthlyCheckup
       - SeasonalCheckup
       - PreventiveCheckup
       - EmergencyCheckup
     - SpecialCare
       - PostPregnancyCheckup
       - InjuryTreatment
       - DiseaseDiagnosis
   - Vaccination
     - DiseasePrevention
       - FMDVaccine
       - BrucellosisVaccine
       - BovineTBVaccine
       - AnthraxVaccine
     - YoungAnimalVaccination
       - CalfVaccination
       - KidGoatVaccination
       - LambVaccination
       - BuffaloCalfVaccination
     - SeasonalVaccination
       - WinterVaccination
       - SummerVaccination
       - RainySeasonVaccination
       - DiseaseOutbreakVaccination

5.  WasteManagement 
   - ManureHandling
     - WasteTreatment
       - SolidManureStorage
       - LiquidManureStorage
       - CompostingManure
       - FertilizerProcessing
     - BiogasProduction
       - SmallScaleBiogas
       - LargeScaleBiogas
       - MethaneExtraction
       - EnergyConversion
   - WastewaterTreatment
     - FiltrationAndPurification
       - SedimentationProcess
       - ActivatedCarbonFiltration
       - ReverseOsmosisPurification
       - UVSterilization
     - ChemicalAndBiologicalTreatment
       - pHTreatment
       - BacterialDecomposition
       - ChemicalNeutralization
   - SolidWasteManagement
     - RecyclingAndReusability
       - MetalScrapReprocessing
       - OrganicWasteRecycling
     - DisposalAndIncineration
       - ControlledBurning
       - HazardousWasteDisposal

6.  Equipment 
   - MilkingMachine
     - MilkingTech
       - ClusterMilkingSystem
       - RoboticMilkingUnit
       - SemiAutomaticMilker
       - PipelineMilkingSystem
     - StorageSystems
       - BulkMilkCoolingTanks
       - TemperatureControlledStorage
       - MobileCoolingUnits
       - AutomatedPasteurizers

7.  RecordKeeping 
   - AnimalHealthRecords
     - VeterinaryRecords
       - VeterinaryDiagnosisRecords
       - MedicationHistoryLogs
       - TreatmentEffectivenessReports
       - EmergencyMedicalNotes
     - HealthMonitoring
       - DiseaseTrackingLogs
       - GrowthAndDevelopmentRecords
       - NutritionLogs
       - BreedingHistory
   - MilkProductionRecords
     - DailyAndMonthlyLogs
       - DailyProductionLogs
       - MonthlyProductionSummaries
       - PerAnimalMilkYield
       - ProcessingPlantSupplyRecords
     - QualityAndTestingReports
       - BacterialTestingRecords
       - ChemicalAnalysisLogs
       - FatAndProteinContentReports
       - AdulterationCheckLogs
   - FinancialAndSalesReports
     - RevenueAndExpenses
       - DairyRevenueReports
       - FeedAndEquipmentExpenses
       - EmployeeSalaryRecords
       - UtilityAndMaintenanceCosts
     - SalesAndSupplyTracking
       - WholesaleMilkSalesLogs
       - DairyProductDistribution
       - CustomerOrderHistory
       - SupplyChainReports

## Properties

 ## Object Properties
-  hasPart : Links equipment to its components.
-  produces : Links a milking process to the storage facilities it produces.
-  consumes : Links livestock to the feeding system it consumes.
-  isPartOf : Links a component to the equipment it belongs to.
-  isProducedBy : Links storage facilities to the milking process that produced them.
-  isConsumedBy : Links a feeding system to the livestock that consumes it.
-  hasHealthRecord : Links livestock to its health records.
-  hasMilkingProcess : Links livestock to the milking process it undergoes.
-  hasFeedingSystem : Links livestock to the feeding system it uses.
-  hasStorageFacility : Links a milking process to the storage facilities it uses.
-  hasQualityControl : Links storage facilities to quality control tests.
-  hasWasteManagement : Links waste management processes to waste treatment methods.
-  hasEquipment : Links a milking process to the equipment it uses.
-  hasRecord : Links record-keeping systems to veterinary records.
-  hasVaccination : Links livestock to the vaccinations it receives.
-  hasTest : Links quality control to bacterial testing.
-  hasTreatment : Links animal health to injury treatment.
-  hasSupplement : Links livestock to the supplements it receives.
-  hasFodder : Links livestock to the fodder it consumes.
-  hasCheckup : Links livestock to veterinary checkups.

  ## Data Properties
-  hasName : The name of the livestock or equipment (domain: Livestock, Equipment).
-  hasAge : The age of the livestock (domain: Livestock, range: xsd:integer).
-  hasWeight : The weight of the livestock (domain: Livestock, range: xsd:decimal).
-  hasMilkYield : The milk yield of a dairy cow (domain: DairyCow, range: xsd:decimal).
-  hasVaccinationDate : The date of vaccination (domain: Vaccination, range: xsd:date).
-  hasProductionDate : The date of milk production (domain: MilkProcessing, range: xsd:date).
-  hasStorageTemperature : The temperature of storage facilities (domain: StorageFacilities, range: xsd:decimal).
-  hasTestResult : The result of a quality control test (domain: QualityControl, range: xsd:string).
-  hasWasteVolume : The volume of waste (domain: WasteManagement, range: xsd:decimal).
-  hasCost : The cost of equipment (domain: Equipment, range: xsd:decimal).
-  hasSupplementDose : The dose of a supplement (domain: SupplementaryFeeding, range: xsd:decimal).
-  hasFodderQuantity : The quantity of fodder (domain: FodderManagement, range: xsd:decimal).
-  hasCheckupDate : The date of a veterinary checkup (domain: VeterinaryCheckup, range: xsd:date).
-  hasFatContent : The fat content of milk (domain: DairyCow, range: xsd:decimal).
-  hasProteinContent : The protein content of milk (domain: DairyCow, range: xsd:decimal).
-  hasLactoseContent : The lactose content of milk (domain: DairyCow, range: xsd:decimal).
-  hasEnergyOutput : The energy output of biogas production (domain: BiogasProduction, range: xsd:decimal).
-  hasEmployeeCount : The number of employees (domain: FinancialAndSalesReports, range: xsd:integer).

## Individuals (Instances )

The ontology includes specific instances to illustrate the concepts:

 # Livestock Instances
-  Daisy : A JerseyCow with name "Daisy", age 5, weight 600.5, milk yield 25.3, fat content 3.8, protein content 3.2, lactose content 4.7.
-  Bella : A HolsteinCow with name "Bella", age 4, weight 700.0, milk yield 30.0, fat content 4.0, protein content 3.5, lactose content 4.9.
-  Max : An AngusCow with name "Max", age 6, weight 800.0.
-  Luna : A MurrahBuffalo with name "Luna", age 7, weight 900.0, milk yield 20.0, fat content 7.5, protein content 4.0, lactose content 5.2.
-  Charlie : A SaanenGoat with name "Charlie", age 3, weight 50.0, milk yield 5.0, fat content 4.5, protein content 3.0, lactose content 4.3.
-  Rocky : A BoerGoat with name "Rocky", age 4, weight 60.0.

 # MilkingProcess Instances
-  MilkingMachine1 : A MilkingMachine with name "Milking Machine 1" and cost 5000.0.
-  RoboticMilkingArm1 : A RoboticMilkingArm with name "Robotic Milking Arm 1" and cost 10000.0.
-  ParallelParlor1 : A ParallelParlor with name "Parallel Parlor 1" and cost 8000.0.

# FeedingSystem Instances
-  Feed1 : A GrassFodder with name "Fresh Grass Fodder" and quantity 1000.0.
-  Feed2 : An AlfalfaHay with name "Dried Alfalfa Hay" and quantity 500.0.
-  CalciumSupplement1 : A CalciumSupplements with dose 50.0.
-  VitaminASupplement1 : A VitaminA with dose 10.0.

 # AnimalHealth Instances
-  Vaccine1 : An FMDVaccine with name "FMD Vaccine 2023" and vaccination date "2023-10-01".
-  Checkup1 : A RoutineCheckup with name "Monthly Checkup Oct 2023" and checkup date "2023-10-05".
-  Treatment1 : An InjuryTreatment with name "Injury Treatment Oct 2023" and checkup date "2023-10-15".

 # StorageFacilities Instances
-  StorageTank1 : A BulkMilkStorage with name "Storage Tank 1" and storage temperature 4.0.
-  MobileCoolingTank1 : A MobileCoolingTanks with name "Mobile Cooling Tank 1" and storage temperature 2.0.

 # QualityControl Instances
-  QualityTest1 : A BacterialTesting with name "Coliform Test 1" and test result "Negative".
-  QualityTest2 : A ChemicalTesting with name "Fat Content Test 1" and test result "3.5".

 # WasteManagement Instances
-  Waste1 : A SolidManureStorage with name "Manure Storage 1" and waste volume 1000.0.
-  Waste2 : A CompostingManure with name "Composting Unit 1" and waste volume 500.0.

  # RecordKeeping Instances
-  Record1 : A VeterinaryRecords with name "Daisy's Health Record".
-  Record2 : A MilkProductionRecords with name "Bella's Milk Log".
-  Record3 : A FinancialAndSalesReports with name "October 2023 Sales Report" and employee count 10.
