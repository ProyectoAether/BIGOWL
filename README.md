
# BIGOWL

BIGOWL (BIG data analytics OWL2 ontology) acts as a formal schema for representing and consolidating knowledge in Big Data analytics. Knowledge incorporation is, in turn, beneficial for efficient algorithmic performance by taking part in the operator’s design, parameter selection, and human interactive and decision-making strategies.

BIGOWL ontologies family is composed of the following ontologies

 - **BIGOWLData**. This ontology contains all the classes and properties related to data. _Data_ is devoted to annotating all the data flowing throughout the analytic workflow. It is declared as _EquivalentTo IO-Class_ of DMOP. This aligning enables datatypes defined by third parties’ ontologies to be contextualised in the analysis.  BIGOWLData contains the main data properties defined for this class, namely: _path_, to annotate the origin of data; and _hasDataType_, which establishes the relationship with class _DataType_. This last is used to define the data type, i.e. _PrimitiveType_ (Double, Integer, Boolean, etc.) or _StructuredType_ (Graph, Tree, Matrix, Vector, Tuple, etc.).
 - **BIGOWLProblems**. It is used to represent the problem class and its properties. Problem is oriented to the specific problem domain (Smart Cities, Biology, etc.).
 - **BIGOWLAlgorithms**. This ontology covers all possible kinds. It has two main subclasses: _DataMiningAlgorithm_ and _OptimizationAlgorithm_, which are used to distinguish between these two families of algorithms. The former is included in the form of equivalence with the class _DM-Algorithm_, which is linked from DMOP.
 - **BIGOWLWorkflows**. It is used to guide the correct orchestration of a workflow, including elements like tasks, components, parameters, etc. This ontology imports BIGOWLData and BIGOWLAlgorithms to define all the pieces in a workflow.
