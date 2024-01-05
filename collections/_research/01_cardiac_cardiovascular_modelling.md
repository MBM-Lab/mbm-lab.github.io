---
layout: sub_research_page
title: "Computational Bodily Fluids and Cardiac Modelling"
description: "The computational bodily fluids group focuses on modeling applied to the quantitative description of the movement of bodily fluids and their interaction with blood vessels and other tissues. The main areas of research are twofold: (i) the construction of highly detailed computational models for studying fundamental questions regarding the physiology and pathology of the cardiovascular system and related systems, and (ii) the study of specific clinical problems that arise in hospital settings (in collaboration with DICAM and DISI). Currently, we collaborate with three local hospitals (S. Maria del Carmine Hospital in Rovereto, Santa Chiara Hospital in Trento, and Civil Hospital in Arco) on various projects, as well as with St. Olav University Hospital (Trondheim, Norway). These models require the discretization of partial and ordinary differential equations in one or more spatial dimensions with complex geometries, as well as the integration of patient-specific data."
# table of contents
toc:
    research1:
      title: "Computational Bodily Fluids"
      anchor: "computational-bodily-fluids"
      imgLink: "/assets/adavn.png"
      contact: Prof. Müller
    research2:
      title: "Cardiac Modelling"
      anchor: "cardiac-modelling"
      imgLink:
      contact: Prof. Pezzuto
---

## Computational Bodily Fluids

### Description

We are interested in the description of bodily fluids dynamics by means of mathematical models and in the design of efficient numerical methods to obtain accurate and robust approximations of their solutions. We want to answer questions regarding basic cardiovascular physiology and pathology, as well as their link to disease and their impact on other processes such as neurovascular physiology and pathology. We also carry on projects closely linked to the clinic, involving intense dialogue with clinicians from local and international hospitals. All these applications are tackled using mathematical models that describe the underlying physical processes, and numerical methods needed to resolve the mathematical models.



### Global models for cardiovascular physiology

We have developed very complex models for the cardiovascular system, including large networks of arteries and veins, as well as other components of the cardiovascular systems. These models are rather unique, especially the one developed with Prof. Eleuterio Toro (University of Trento, Italy) since 2014, as well as a newer and more complex model developed in collaboration with Prof. Blanco (National Laboratory for Scientific Computing, Brazil). Besides representing an excellent scenario for developing numerical schemes for hyperbolic PDEs on networks, they are the backbone on which we are building an in-silico “physiology lab” for the study of many aspects of cardiovascular physiology that are still unclear. Our modeling effort regards also the CerebroSpinal Fluid (CSF) and its interaction with blood vessels, as well as the lymphatic system. This project also involves the need to use experimental data, and thus to adopt and develop data assimilation tools and to interact with laboratories that gather physiological data. This project is a distinctive aspect of our research group and focuses on understanding physiology rather than on concrete medical applications.

![alt](/assets/GM2-eps-converted-to.png)

![alt](/assets/adavn.png)

Overview of a global model for human circulation and CSF/brain dynamics (top) and of the Anatomically Detailed Arterial-Venous network model (bottom). Images taken from [this](https://doi.org/10.1002/cnm.3532) and [this paper.](https://doi.org/10.3389/fphys.2023.1162391)

#### Assessing the interaction of cerebral blood flow, cerebrospinal fluids and brain dynamics.

We have coupled our blood flow model to a model for cerebrospinal fluid and brain dynamics, which allows us to study the interaction of all these components. We have used this model to describe the impact of venous strictures located in the neck, on intracranial haemodynamics. We are also trying to unveil which are the major determinants of the intracranial pressure waveform.

####  Improvement of models of cerebral venous flow

A crucial role in cerebral perfusion is played by intracranial pressure, which is considered the downstream pressure in cerebral perfusion. This is due to the fact that cerebral veins collapse in correspondence to the point where they merge to dural venous sinuses. The model that we are currently using to describe this phenomenon is rather simplistic and does not reproduce the increase in resistance at the collapse point for varying intracranial pressure. The development of a richer model will allow us to reassess many modeling results produced so far.

#### Assessing autonomic nervous system action on venous compliance for arterial pressure control.

The venous system plays a big role controlling mean arterial pressure. In turn, the venous system properties are controlled by the autonomic nervous system. There is interest in understanding better how this control works and how it varies in different parts of the body. We plan to work with our global circulation model, in combination with experiments on animals to better characterize the interaction of the ANS and the venous system, having in mind as application the development of better ways to treat hypertension.

#### Modeling orthostatic stress

Virtually no one has modeled orthostatic stress with 1D models for venous blood flow. We are working in that direction, with many challenges to be faced. The project here would regard a first approach to this problem and would regard the reparametrization of currently available vessel models, as well as most probably the reparametrization and enrichment of control mechanisms currently included in our model.

#### Modeling the cardiorespiratory system

While the modeling of transport and exchange of species is rather well-established from a theoretical point of view, our global models currently do not include such aspects. We are transferring existing knowledge available in physiology as well as in the modeling literature, to our complex vascular models, aiming at incorporating metabolism and respiratory dynamics as driving forces for blood flow.

#### Modeling the lymphatic system

Blood and cerebrospinal fluid are not the only fluids in the body. From the many other fluids present in our body, the lymph is of paramount importance in the onset and progression of pathological states. We are working on mathematical models that are specific for the lymphatic system, aiming at a coupling of this system to other systems already present in our modeling framework.

### Non-invasive estimation of haemodynamic indexes

This research topic brings us very close to the clinic. The aim here is to reproduce haemodynamic indexes that are normally acquired via invasive measurements, by using medical imaging and mechanistic models. This is a complex task which involves strong interaction with clinicians, securing the necessary data to develop a methodology and the clinical validation of the resulting method.

![alt](/assets/mlffr.png) -->

Pipeline for non-invasive machine learning- and model-based Fractional Flow Reserve prediction. Image taken from [this paper.](https://doi.org/10.1016/j.cma.2021.113892)

####  Non-invasive estimation of FFR

Fractional Flow Reserve (FFR) is the gold standard method to determine how a stenotic coronary artery should be treated. Our most active project on this front regards a collaboration with Prof. Leif Hellevik’s group at the Norwegian University of Science and Technology (NTNU Trondheim, Norway) on the development of non-invasive methods to estimate hemodynamic indexes used in cardiology. Our collaborators at NTNU have created a large database of patients with stable coronary artery disease and together we have developed a pipeline to non-invasively estimate an index that is normally measured using a pressure sensor that is inserted into the coronary arteries and that requires the use of drugs to elicit maximal blood flow to the heart muscle.

####  Defining the best model pipeline for iFR

iFR is an index for assessing the functionality of coronary artery disease. It is emerging as a valid alternative to FFR and it is attractive because it does not require to induce hyperemia. In this project we explore which is the best modeling pipeline for iFR estimation by means of the design of the pipeline and then parameter selection and optimization. By pipeline we mean the set of sequential decisions that, departing with a medical image, result in a final iFR estimation. The pipeline requires also to select which fluid model should be used: 1D/0D or 3D, transient or steady state, including machine learning for having fast and accurate reduced-order models?


### Cerebral haemodynamics and waste clearance

This is a project related to fluid exchange in the brain. This is a very active area of research in human physiology, since it is postulated that deficiencies in waste clearance mechanisms could be at the basis of many neurodegenerative diseases. We are interested in the coupling of pulsating blood and the surrounding tissue, as well as in the effect that pulse wave propagation has on brain-specific structures that are considered as potentially crucial pathways for fast transport in the brain.

![alt](/assets/corner_tree_t1.png)

Impact of blood pressure pulse propagation in the deformation of elastic tissue to model mechanical coupling phenomena in vascularized tissues. Image taken from [this paper.](https://doi.org/10.1007/s10439-021-02804-0)


####  Mechanical coupling of 1D blood flow in vessels and 3D tissue

Vascularized tissue can be seen as 1D structures that deform within a 3D tissue. Being able to model this behavior at such scale has not been done previously and could pave the road for homogenized models that are based on a deep understanding of the smaller scale interactions between vessels and tissue. Collaborators from SISSA and WIAS institute have worked out a theoretical model for the study of this coupled problem and we are now working on the coupling of our 1D blood flow solvers with their 3D mechanical model (so far linear elastic). The implications of this work are various, including the improvement of models used in the identification of mechanical properties of tissue using medical images, as well as a better understanding of transport processes in vascularized tissues.

#### PVS flow in complex networks

The transport of substances in the so-called perivascular spaces of cerebral arteries and veins is part of a larger debate about transport mechanisms in the brain. Here we aim at constructing on top of previous work on co-axial flow models with the goal of assessing how the perivascular-space flow acts when we model not a single vessel but a network of vessels, enhancing thus our capacity to properly describe the interaction of arterial pressure waveforms and such flow.

Combining wearables and mechanistic models for remote patient-monitoring: this is a project involving our research group and Prof. Riccardi's group (DISI, UNITN) as partners. The project proposes to construct and deploy wearables on patients with cardiac and respiratory diseases so that they are remotely monitored. Mathematical modeling will be used to assess the quality of the data. We will also investigate the capacity of models to, in combination with wearable-acquired data, reproduce variables that are normally only accessible when the patient visits the hospital. This is an ongoing topic in which we collaborate with the cardiology department of Santa Chiara hospital (headed by Dr. Bonmassari) and the Pneumology department of the Ospedale Civile di Arco (headed by Dr. Nardelli).

### Numerical methods for hyperbolic conservation laws on networks

This research topic is deeply rooted in our group since our main fields of work are numerical analysis and scientific computing. We have specialized over time on designing numerical methods that perform well for the modeling of problems that our group approaches. In particular, since we mainly work with network models in which flow dynamics are described by one-dimensional models, we have focused on the development of numerical methods for hyperbolic (or hyperbolic-dominant) partial differential equations applied on networks of one-dimensional domains and possibly coupled to geometrically heterogeneous models arising from the need to couple vascular models to peripheral circulation models or surrounding tissues.

![alt](/assets/ref_p_4.png)

Propagation of a pressure wave over a network of vessels (vertical dashed lines show bifurcation points) computed using different modelling and numerical strategies. Image taken from [this paper.](https://doi.org/10.1016/j.jcp.2016.03.012)

#### Robust numerical methods for variable properties and collapse

When modeling orthostatic stress or the effect of external pressure on vessels ends up dealing with extreme situations. In such cases one wants to have numerical methods with certain properties, in particular the ability to deal with collapse. Another desirable property is that it correctly deals with steady state solutions, including difficulties arising when vessel properties vary in space and when friction terms are to be considered.

#### Efficient numerical methods for hyperbolic conservation laws on networks

Dealing with large vascular models implies that spatial scales can vary considerably. Moreover, considering blood pressure control or the interaction of different body fluids (for example blood and cerebrospinal fluid, blood and lymph, blood and transported gasses) might result in very different time scales. The numerical strategies used to solve models with these properties have to be efficient, which implies they have to offer an optimal tradeoff between accuracy and computational cost. It is well known that this is often achieved with high-order numerical methods. We have so far explored efficient explicit time discretization strategies, their parallelization using shared- and distributed memory parallel computing, as well as the capacity to adaptively select the model to be used. We are currently exploring PDE splitting strategies, and are also interested in exploring alternative discretization strategies, including implicit time discretization schemes.

#### Enriched 1D blood flow models

Departing from the supine position means modeling large deformations. We propose here to consider additional terms in one-dimensional blood flow models, arising from axial deformation or tethering, as well as from the presence of surrounding tissue, or even to the fact that collapse can be required to model localized pressure losses with distributed models. One-dimensional models can also be enriched by considering extended models that provide a more accurate description of the velocity profile at a given cross-section. All these aspects, and many others, will result in alternative systems of PDEs. Consequently, adopted numerical discretization strategies will need to be adapted.

#### Knowledge transfer to other applications.

The methods developed so far have been always applied to blood flow problems. However, the methodology is general and can be applied to similar problems which involve hyperbolic conservation laws on networks, such as traffic flow, gas and oil transport, water distribution, sewage collection, to name just a few.


### Main collaborations.

These are our current main collaborators:

#### National collaborators applied mathematics and modeling

* DICAM, University of Trento. We collaborate with Prof. Fraccarollo and Prof. Siviglia on blood flow modelling and on the development of numerical methods.
* DICCA, University of Genova. We collaborate with Prof. Repetto on ocular fluid dynamics and its interaction with the cardiovascular system. Prof. Repetto has also other research interests for which he can suggest master thesis projects.
* MOX, Polimi, Milan. We collaborate with Prof. Vergara on coronary blood flow modelling.
* SISSA, Trieste. We collaborate with Prof. Heltai on the mechanical coupling of dimensionally heterogeneous models.
* University of Padova. Collaboration with Prof. Susin and colleagues on different projects regarding valve dynamics and extracorporeal membrane oxygenation.

#### International collaborators applied mathematics and modeling

* Weierstrass Institut, Berlin, Germany. We collaborate with Dr. Caiazzo on the mechanical coupling of dimensionally heterogeneous models. We have previously collaborated on the development of parameter estimation techniques.
* Department of Mathematics, Malaga, Spain. We collaborate with Prof. Parés on the development of numerical methods for hyperbolic PDEs.
* King's College, London, UK. We collaborate with Prof. Alastruey on the application of one-dimensional blood flow modeling to study cardiovascular physiology and pathology.

#### Local hospitals
* Santa Chiara Hospital (Trento, Italy). We are in contact/collaborate with the cardiology department, in particular with its head, Dr. Bonmassari, and some of his collaborators.
* Rovereto Hospital (Rovereto, Italy). We are in contact/collaborate with the otorhinolaryngology department of the Rovereto Hospital (headed by Dr. Frau).
* Arco Hospital (Arco, Italy). We are in contact and plan to establish a collaboration with the pneumology department, headed by Dr. Nardelli.


#### International collaborators in biomedical research

* Wayne State University (Detroit, USA): we have collaborated since 2013 with Dr. Haacke, an MRI physicist interested in the imaging of the brain and its vasculature.
* Norwegian University of Science and Technology (NTNU, Trondheim, Norway): we collaborate with the cardiology and radiology departments of the university hospital (St. Olav’s hospital).
* Bioengineering Institute (Auckland, New Zealand): we collaborate with Dr. Maso Talou on the modeling of blood pressure control mechanisms and with Dr. Reynolds on modeling of the lymphatic system.
* The Pennsylvania State University, Department of Engineering Science and Mechanics (USA): we collaborate with Prof. Francesco Costanzo on peri-vascular cerebral flow models.

### Thesis proposals

Please contact [Prof. Müller](https://webapps.unitn.it/du/it/Persona/PER0027674/Pubblicazioni) if you are interested in research projects regarding possible topics for your master thesis or our PhD in applied mathematics.

---

## Cardiac Modelling

Pezzuto’s group activities lie at the intersection of mathematical biology, numerical analysis, and human physiology. Organ-scale models, such as for the heart, require special care in developing effective numerical schemes for their simulation. Cardiac models are multi-physics and multi-scale, and their simulation requires supercomputers. Therefore, the group is developing novel multi-fidelity approaches based on scientific machine learning and simplified physics (e.g., the eikonal equation) for real-time simulation of cardiac models.

Fast and accurate models are fundamental for collaboration with clinicians and physiologists. Clinical applications, such as atrial fibrillation and cardiac resynchronization therapy, are a valuable source of problems of interest. Since cardiac modeling genuinely lies at the intersection between applied mathematics and cardiology, topics also require strong interdisciplinary competencies, secured over the years through collaborations with scientists of diverse disciplines.

### Physics-Informed Learning

Physics-Informed Neural Networks (PINNs) is a powerful tool for solving inverse and parametric problems. With PINNs, we can estimate the cardiac conduction velocity and fibers from clinical recordings. More generally, Scientific Machine Learning provides new tools for approximating complex parameter-to-solution maps in PDE problems. One challenge is to apply these tools to complex domains like cardiac anatomy. For instance, we developed a Gaussian Process Regression method to work on manifolds, which enables classification and learning on the human atria.

### Inverse Problems

The current grand challenge in cardiac modeling is individualizing complex, yet generic models of cardiac electrophysiology (EP) to the pathophysiology of the patient. In this direction, our group made a significant step forward towards EP personalization with either non-invasive or minimally-invasive clinical data.

Non-invasive ventricular activation reconstruction from the 12-lead ECG and CMR has been demonstrated in a heterogeneous cohort of patients. The algorithm overcomes the severely ill-posedness of the inverse problem by employing an accurate, fast-to-simulate forward ECG model, based on the eikonal equation, and with physiologically grounded parameters.

Non-invasive assessment of the local conduction velocity in the atria has been approached as a PDE-constrained optimization problem. Here, we can estimate the full conductivity tensor, which also defines the fiber direction, from sparse recordings of cardiac activation. The method has also been applied in the clinical context.

The identification of the sites of earliest activation from the 12-lead ECG has been formulated in terms of geodesic paths. In this way, we can easily compute sensitivities, even on complex geometries. The problem is also challenging because the number of sites is generally unknown. We, therefore, proposed a topological gradient to incrementally add new sites.

### Uncertainty Quantification

Uncertainty is inevitable in dealing with clinical data. Patient-specific models should therefore provide a quantitative estimate of the uncertainty in predictions. Our group uses multi-fidelity and multi-level methods to enable accurate UQ for complex cardiac models with high-dimensional random variables without compromising computational efficiency. We specifically considered physics-based low-fidelity models that, oppositely to standard surrogate models, can cope with high-dimensional uncertainty without an extensive training phase.

### Atrial Fibrillation

Atrial Fibrillation (AF), the most common cardiac arrhythmia, is a chaotic spatiotemporal activation of the atria. Computer models can greatly help our pathophysiological understanding and clinical management of AF, yet we are still far from capturing the full complexity of the disease. We have access to one of the most advanced models of the human atria, and we are working to further improve it in the future. The model is structurally and physiologically accurate. We can simulate physiologically-grounded scenarios of AF, including the surface ECG.

### Active Mechanics

Active materials undergo deformations also in absence of mechanical stresses. Examples include cardiac contraction and relaxation, tumor growth, and morphogenesis. Mechanically, the macroscopic deformation is dictated by a microstructural distortion, combined with an elastic relaxation. In this way, we can model inelastic phenomena and then use them to derive the equations of motion. Active strain is an effective approach in this respect. For instance, in a solid tumor, we can account for the effect of external pressure on tumor growth.

### Software

We develop and maintain several software packages for the simulation of cardiac electrophysiology, such as Propeiko and Propag-5. Propag-5 is a well-established software capable of simulating large-scale problems, such as those arising in atrial fibrillation, on supercomputing centers by exploiting multiple nodes via MPI, multiple cores via OpenMP and GPU accelerators with CUDA. Propeiko is a fast ECG simulator based on the anisotropic eikonal equation and lead field formulation of the forward bidomain model. Propeiko runs almost real-time on GPU, enabling interactive solution and fast uncertainty quantification and parameter inference. Moreover, it compares favorably to high-fidelity
simulations with the full, time-consuming reaction-diffusion EP model.

### Thesis proposals

Please contact [Prof. Pezzuto](https://webapps.unitn.it/du/it/Persona/PER0251606/Curriculum) if you are interested in research projects regarding possible topics for your master thesis or our PhD in applied mathematics.
