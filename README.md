# Metad_ML
Machine learning code to build model for most effective CV for metadynamics simulations, using initial trajectories.
The code is made of a basic Tensorflow setup that can be run locally or on google colab (latter preferred).
The input file is supposed to be a trajectory file converted into a pdb with only protein atoms. These atoms will be extracted to define features.
By default, the features to be defined will be the phi and psi angles. Users can suggest additional features to use for ML model building.

For the current example, the label has been manually defined to be "a1", the angle between com1, com2 and com3, where com=centre of mass for a defined bunch of atoms. The angles can be obtained from the HILLS or the COLVAR (if made) file generated during a Plumed metadynamics run. For the current example, two columns, the first for time and the second for a1 will be used for input as a csv file.

The rest will be updated as the project goes further.
