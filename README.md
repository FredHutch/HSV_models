# HSV_models
This repository supports multiple stochastic HSV models written in C++ by collecting key files required
to build them on a Linux UBUNTU 3.3 platform.  In particular it supports models that require GTK 2.0 
and OpenGL for their graphical output. Some of the models can be compiled without the GUI interface 
and would not require the files in this repository.  

Since the required packages may not be available on current systems, this repository should be cloned
and the path to the extra_libs subdirectory must be set as the value of the GTKGLEXT environment 
variable before running make in the Linux directory.  It is preferable that users download the 
gtkglext package for their system, but we replicate the binary library files and headers of the
versions originally used here in case they are no longer available.

The models wll be available in separate git repositories listed below.
In general, they fall into two classes: compartmental ODE and agent-based models.
All models have spatial components.  


HSV_ODE_model1 - the first model written for these papers

    Rapid localized spread and immunologic containment define herpes simplex virus-2 reactivation in the human genital tract,Elife,Schiffer,et al,2013
    Rapid Viral Expansion and Short Drug Half-Life Explain the Incomplete Effectiveness of Current Herpes Simplex Virus 2-Directed Antiviral Agents,
        Antimicrobial Agents and Chemotherapy, Schiffer,et al,2013
    Herpes simplex virus-2 transmission probability estimates based on quantity of viral shedding,
        Journal of The Royal Society Interface, Schiffer,et al,2014

 - This model requires the graphics libraries.  You may also need to load the Mesa module to compile and run it.

HSV_ODE_model2 - this is an enhancement of the first model written for these papers

    Increased herpes simplex virus-2 shedding in hiv-1 infected persons is due to poor immunologic control in both ganglia and genital mucosa,
	Sexually Transmitted Infections,Schiffer,et al,2015

    Mathematical modeling of herpes simplex virus-2 suppression with pritelivir predicts trial outcomes, 
        Science translational medicine,Schiffer,et al,2016

    A Fixed Spatial Structure of CD8 + T Cells in Tissue during Chronic HSV-2 Infection,
	Journal of Immunology, Schiffer,et al,2016

 - This model can be compiled with or without the GUI (and associateds libraries).  

HSV_AGENT_model1 - this is an agent-based implementation that eventually led to the paper

    Tissue-resident T cell derived cytokines eliminate herpes simplex virus-2 infected cells,
        The Journal of clinical investigation,Roychoudhury,et al,2020
