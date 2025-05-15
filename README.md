
The **Dairy Farm Ontology (DFO)** models dairy farming operations, including livestock management, feeding systems, milking processes, waste handling, and quality control. It addresses earlier inconsistencies (e.g., misuse of superclasses, incorrect hierarchies) and provides a logically consistent framework for semantic reasoning.

---

## Key Features
- **Classes**: So Many classes covering livestock, equipment, health management, and waste treatment.
- **Object Properties**: Relationships like `hasLivestock`, `usesFeedingSystem`, and `hasQualityControl`.
- **Data Properties**: Track milk yield, vaccination dates, equipment costs, and feed quantities.
- **Individuals**: Pre-populated instances (e.g., cows, goats, milking machines, vaccines).
- **Reasoner-Ready**: Validated with HermiT for consistency.

---

## Ontology Overview
![Class Hierarchy Diagram](assets/class_diagram.png)  
*(Generated using [Protégé OntoGraf](https://protege.stanford.edu/))*  

### Core Classes
- **DairyFarm**: Central class linking all components.
- **DairyAnimalStock**: Subclasses for cows, buffaloes, goats.
- **FarmEquipment**: Milking machines, storage tanks.
- **DiseasePreventionProgram**: Vaccination schedules.
- **WasteHandling**: Manure treatment and recycling.

---

