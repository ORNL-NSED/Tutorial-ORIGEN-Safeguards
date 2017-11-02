# Tutorial-ORIGEN-Safeguards

This repository contains materials for SCALE/ORIGEN 6.2 tutorials at ANS Winter 2017 with a focus on Nuclear Non-proliferation and Safeguards.

The latest SCALE 6.2 may be obtained from [RSICC](https://rsicc.ornl.gov/PackageDetail.aspx?p=SCALE%206.2.1&id=C00834&cpu=MNYCP&v=02&t=A%20Comprehensive%20Modeling%20and%20Simulation%20Suite%20for%20Nuclear%20Safety%20Analysis%20and%20Design;%20Includes%20ORIGEN%20and%20AMPX.). Details about SCALE and information about training courses may be found on the [SCALE website](https://www.ornl.gov/scale).

## Contents

The material in this repository is summarized as follows.

* [`docs/`](https://github.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/tree/master/docs/) documentation
    * [`scale62_origen.pdf`](https://github.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/blob/master/docs/scale62_origen.pdf) only the ORIGEN section from the manual
    * [`presentations/`](https://github.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/tree/master/docs/presentations/) additional presentations
        * [`SCALE_workshop_2017_Hu.pdf`](https://github.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/blob/master/docs/presentations/SCALE_workshop_2017_Hu.pdf) SCALE Users' Group 2017 presentation on ORNL applications with ORIGAMI
        * [`ORIGEN_tutorial_ANS_2017.pdf`](https://github.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/blob/master/docs/presentations/ORIGEN_tutorial_ANS_2017.pdf) presentation for ANS Winter 2017
        * [`2017_SCALE_UsersGroup_ORIGEN61to62.pdf`](https://github.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/blob/master/docs/presentations/2017_SCALE_UsersGroup_ORIGEN61to62.pdf) SCALE Users' Group 2017 on changes to ORIGEN from SCALE 6.1->6.2
* [`src/`](https://github.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/tree/master/src/) annotated code inputs
    * [`decay/`](https://github.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/tree/master/src/decay/) various decay-only problems
        * [`decay.inp`](https://raw.githubusercontent.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/master/src/decay/decay.inp) starter input for decay of U-238
        * [`u238.inp`](https://raw.githubusercontent.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/master/src/decay/u238.inp) final model for decay of U-238 and calculation of Rn-222 for 1 billion years
        * [`puo2.inp`](https://raw.githubusercontent.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/master/src/decay/puo2.inp) emission spectra of plutonium oxide
        * [`puc.inp`](https://raw.githubusercontent.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/master/src/decay/puc.inp)  emission spectra of plutonium carbide
        * [`template.inp`](https://raw.githubusercontent.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/master/src/decay/template.inp) a template for decay calculations with emissions
    * [`snf/`](https://github.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/tree/master/src/snf/) how to use ORIGEN reactor libraries for spent fuel isotopics calculation
        * [`fuel.inp`](https://raw.githubusercontent.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/master/src/snf/fuel.inp) Basic ORIGAMI input
        * [`w17_ax.inp`](https://raw.githubusercontent.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/master/src/snf/w17_ax.inp) ORIGAMI input with 3 axial nodes
        * [`restart_decay.inp`](https://raw.githubusercontent.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/master/src/snf/restart_decay.inp) transfer isotopics from ORIGAMI in ORIGEN for decay
        * [`restart_emit.inp`](https://raw.githubusercontent.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/master/src/snf/restart_decay.inp) transfer isotopics from ORIGAMI in ORIGEN for emission calculations
        * [`w17_ax.inp`](https://raw.githubusercontent.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/master/src/snf/origami_ge10x10.inp) ORIGAMI input with 3 axial nodes        
        * [`origami_ge10x10.inp`](https://raw.githubusercontent.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/master/src/snf/origami_ge10x10.inp) General Electric 10x10 gamma emission with ORIGAMI
        * [`origami_w17x17_bu15.inp`](https://raw.githubusercontent.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/master/src/snf/origami_w17x17_bu15.inp) Westinghouse 17x17 Pu content with ORIGAMI at 15 GWd/MTU
        * [`origami_w17x17_bu30.inp`](https://raw.githubusercontent.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/master/src/snf/origami_w17x17_bu30.inp) Westinghouse 17x17 Pu content with ORIGAMI at 30 GWd/MTU
        * [`origami_w17x17_bu45.inp`](https://raw.githubusercontent.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/master/src/snf/origami_w17x17_bu45.inp) Westinghouse 17x17 Pu content with ORIGAMI at 45 GWd/MTU
    * [`shielding/`](https://github.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/tree/master/src/shielding/) 
        * [`origen_to_mavric.inp`](https://raw.githubusercontent.com/ORNL-NSED/Tutorial-ORIGEN-Safeguards/master/src/shielding/origen_to_mavric.inp) load photon source calculated by ORIGEN in MAVRIC


## ANS Winter 2017 Tutorials

Two sessions were organized for ANS Winter 2017 with abstracts below.

### SCALE/ORIGEN for Nuclear Nonproliferation and Safeguards Applications–Tutorial

The ORIGEN depletion and decay code in the SCALE Code System has been internationally used for decades
to predict spent nuclear fuel compositions and radiation emissions that are essential for a broad spectrum
of applications. The new ORIGEN release features a modernized, user-friendly input, with enhanced
autocomplete and results display capabilities under the new SCALE graphical interface. The aim of this
tutorial is to provide an overview of ORIGEN’s capabilities, with a focus on those that directly support
safeguards and nonproliferation applications. Hands-on examples will be included, such as estimation
of uranium and plutonium in spent fuel for material reporting and calculation of neutron and gamma
sources to support spent fuel verification. The tutorial is open to all participants at the conference. No prior
experience with SCALE is required. Participants wishing to follow along with the tutorial should bring their
own computer, have a valid license for SCALE 6.2.1 or the most recent version, and have this SCALE version
installed on their computer.

*This tutorial will focus on the simpler models in `src/decay/` and the ORIGAMI problems in `src/snf/.`*

### SCALE/ORIGEN for Shielding Source Term Generation–Tutorial

The ORIGEN depletion and decay code in the SCALE Code System includes, in addition to isotopic evolution
prediction, the capability to calculate neutron, photon, alpha, and beta decay emissions, commonly used as
time-dependent source terms in shielding calculations. This tutorial will focus on generating source terms
for arbitrary materials. Hands-on examples will be included on generating neutron and photon sources for
irradiated fuel and activated structural components and feeding ORIGEN neutron and photon sources into a
MAVRIC shielding calculation. The tutorial is open to all participants at the conference. Participants wishing
to follow along with the tutorial should bring their own computer, have a valid license for SCALE 6.2.1 or the
most recent version, and have this SCALE version installed on their computer. This tutorial will not include
basic SCALE GUI usage or a broad overview of the ORIGEN input—for this, participants are encouraged to
attend the companion session “SCALE/ORIGEN for Nuclear Nonproliferation and Safeguards Applications”.

*This tutorial will focus on the more complex models in `src/snf/` and `src/shielding/.`*
