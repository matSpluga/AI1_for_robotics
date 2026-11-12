# Automated Assembly Line Ontology

This project develops an ontology describing an automated assembly line for printed circuit board (PCB) manufacturing using Surface-Mount Technology (SMT).

The ontology models the main physical elements of an assembly machine, the component types handled by the machine, and the operations involved in picking, inspecting, positioning, and placing components on a PCB.

## Project contents

- `Group1_ontology.owx` – the OWL ontology containing the classes, object properties, data properties, and logical restrictions used to represent the assembly line. It can be opened and edited with [Protégé](https://protege.stanford.edu/).
- `AI4RO1_Group1_2025_26.pdf` – the project report, describing the domain, design choices, ontology structure, and validation results.
- `Automated-lines-onthology.properties` – ontology-related properties/configuration file.
- `Images/` – figures illustrating the ontology structure and its properties.
- `Papers/` – research papers and supporting material used during the development of the ontology.

## Ontology overview

The ontology represents an SMT assembly line inspired by an automated PCB assembly machine. Its main elements include:

- **Conceptual entities**, such as PCB placements, component types, and unfixable problems detected during inspection.
- **Physical objects**, including the PCB, components, and machine parts such as the magazine rack, placement heads, nozzles, and movement table.
- **Object properties**, describing relationships and operations among these entities, such as gripping, retrieving, inspecting, disposing of, and placing components.
- **Data properties**, including the X and Y coordinates used to represent PCB and component placement positions.

The model includes component types such as resistors, capacitors, and transistors, and distinguishes between large and small nozzles according to the types of components they can handle.

## Validation

The ontology was tested in Protégé using the ELK, HermiT, and Pellet reasoners. According to the project report, all three reasoners classified the ontology as consistent. Additional description-logic queries were used to check inferences about ejected components and nozzle/component compatibility.

## How to open the project

1. Install and launch [Protégé](https://protege.stanford.edu/).
2. Open `Group1_ontology.owx` from the project folder.
3. Inspect the class hierarchy, object properties, and data properties.
4. Run a reasoner (for example, HermiT, ELK, or Pellet, if available in your Protégé setup) to classify and validate the ontology.
5. Refer to `AI4RO1_Group1_2025_26.pdf` for the design rationale and the example competency queries.

## Authors

- Francesco Sisani
- Matteo Spluga
