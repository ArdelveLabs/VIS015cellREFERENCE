# VIS015cellREFERENCE
CELL Generator: REFERENCE

Cell Generator for REFEREENCE USER has options to ontrol Output voltage and accuracy Inputs

**INPUTS***
Inputs are taken from directory "ArdelveNEWproject" Input files are USER and NETLIST USER defines the cell parameters NETLIST defines the connections and voltage ratings

Inputs are taken from directory "ArdelveDesignConfigurations" CELLBio provides the initila cell bio definiton VIS015 defines any process parameters need Outputs

Inputs are taken from directory "ArdelveVerilog" These contain the symbol pin lists for the micro cells
        cellname.v => verilog output that is imported to cadence to create scheamtic and symbol cellname_bio => Cell Bio    cellname_symbol => Symbol that is used when creating top level netlist Setup

ProjectLinks under "ArdelveDesignConfigurations" defiens the paths fall I/O Call

All these files can be found under  AO-COMPLIERfiles

**OUTPUTS***
Verilog   <<CellName.v>>
Bio       <<CellName_bio.txt>>
Symbol    <<CellName_Symbol.txt>>

**FUNCTION CALL****
GenerateVIS015cellREFERENCE(Instance,debug) 
    Instannce must be found in NETLIST and match the cell name call
    debug=0 to not display any debug status flags
