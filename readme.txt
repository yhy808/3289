NEURON mod files for the slow and fast K+ currents from the paper:
Voltage-gated K+ channels in layer 5 neocortical pyramidal neurones from young rats: subtypes and gradients
A. Korngreen and B. Sakmann, J.Physiol. 525.3, 621-639 (2000).

The kinetics.hoc file reproduces Fig.4 and Fig.7 of the paper
using the kinetic parameters as calculated by the authors using
a pharmacological separation of the currents. 
The activation and deactivation currents were simulated
using the voltage clamp values and protocols indicated
in Fig.4B and 7B with a -21mV reversal potential, because of
the 65mM K+ concentration used in the bath.

The parameter C2 on the caption of fig.7 
for the deactivation time constant of the slow current
should be 175.03 instead of 1.15.

The peak conductances have been arbitrary set to values
giving approximately the same current in the simulations
of Figs.4B and 7B.

Under unix systems:
to compile the mod files use the command 
nrnivmodl 
and run the simulation hoc file with the command 
nrngui kinetics.hoc

Under Windows using NEURON 5.1:
to compile the mod files use the "mknrndll" command.
A double click on the simulation file
kinetics.hoc 
will open the simulation window.

Questions on how to use this model should be directed to
michele@pa.ibf.cnr.it
