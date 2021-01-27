[Про дослідження](index.md)

# Quotes from 1
___
The design of telecommunication networks usually comprises three major phases. First, mathematical analysis is carried out and numerical results obtained. During this phase, simple models are used to facilitate calculations. These simple models involve hypotheses that are not realistic, leading to rough performance figures that are valid only as a first approach to the feasibility of the proposed network. Simulation is the second step in the design process before performance can be monitored and measured in the true network. In contrast to the simple models necessary for the mathematical analysis, models used in simulations permit the relaxation of strict adherence to most of the hypotheses assumed in those models. The results obtained by simulation are much closer to the true world than those obtained by analysis. 
___

# Quotes from 2
___
A simulation is an experiment to determine characteristics of a system empirically. It is a modeling method that mimics or emulates the behavior of a system over time. It involves generation and observation of artificial history of the system under study, which leads to drawing inferences concerning the dynamic behavior of the real system.
___
A computer simulation is a discipline of designing a model of an actual or theoretical system, executing the model (an experiment) on a digital computer, and statistically analyzing the execution output. The current state of the physical system is represented by state variables (program variables). Simulation program modifies state variables to reproduce the evolution of the physical system over time.
___
There are two different uses of statistical methods and one use of probabilistic methods in distribution driven simulations. First, the distributions of input random variables such as inter-arrival times, times to failure, service times, times to repair, etc. need to be estimated from real measurement data. 
___

# Quotes from 3
___
Availability assessment approaches are primarily based on measurement and modeling methods. Model-based approaches are fast and relatively inexpensive methods for system availability analysis in comparison with measurement-based methods. System modeling can be accomplished using discrete-event simulation [2, 3], analytical models, or a hybrid of both approaches. Analytical models fall into four main categories [4, 5, 6, 7]: (i) non-state-space models (reliability graph (RelGraph), reliability block diagram (RBG), or fault tree (FT)), state-space models (Markov chains, Stochastic Petri net (SPN), stochastic reward net (SRN), etc.), hierarchical models, and fixed-point iterative models. Non-state-space modeling paradigms provide a relatively quick evaluation of basic metrics for a system (reliability, availability, MTTF) with a proper capture of overall system architecture. State-space models, on the other hand, can capture sophisticated behaviors and operations of a system. This approach can handle failure/repair dependencies and complex interactions between system components. To avoid the largeness problem (or state-space explosion problem) in state-space models, we use hierarchical modeling techniques of non-state-space and state-space models at upper and lower levels, as well as fix-point iterative models. In this chapter, we focus on studying complex system operations in DCs captured by using an SRN.
___

# Quotes from 4
___
The complexity of many real-world systems involves unaffordable analytical models, and consequently, such systems are commonly studied by means of simulation. This problemsolving technique precedes the emergence of computers, but tool and technique got entangled as a result of their development. As defined by Shannon (1975), simulation “is the process of designing a model of a real system and conducting experiments with this model for the purpose either of understanding the behaviour of the system or of evaluating various strategies (within the limits imposed by a criterion or a set of criteria) for the operation of the system.”
___

The simmer package brings discrete-event simulation to R. It is designed as a generic yet powerful process-oriented framework. The architecture encloses a robust and fast simulation core written in C++ with automatic monitoring capabilities. It provides a rich and flexible R API that revolves around the concept of trajectory, a common path in the simulation model for entities of the same type.
___

# Quotes from 5
___

Agent-based Modeling: “An agent is anything that can be viewed as perceiving its environment through sensors and acting upon that environment through effectors.” [17] Furthermore, Macal and North highlight in their paper [18] that agents possess the following characteristics: An agent is (1) identifiable: can be identified by his set of characteristics and rules, (2) situated: is located in an environment and interacts with other agents, (3) goal-directed: is heading forward to achieve a certain objective, (4) autonomous and self-directed: can operate independently in its environment.\
...\
Unified Modeling Language (UML): UML is a standardized graphical modeling language for specifying, visualizing and documenting artifacts of software systems. Furthermore, it can be used for business modeling and non-software systems.\
...\
Graphical Modeling: Graphical models are a combination of probability theory and graph theory. An advantage of these models is that complex systems can be divided into simpler sub-systems. Graphical models can be categorized in directed (e.g. Bayesian network) and undirected graphical (Markov random field) models. [24], [25] Due to their above-mentioned characteristics these models are applied to analyze critical infrastructure interdependencies.\
...\
Of all these approaches the Agent-based Modeling and Simulation (ABMS) approach has proven to be a good way for simulating critical infrastructures and is used in many research projects [13]. ABMS consists of dynamically interacting rulebased agents which reflects the real-world and its complexity [18]. Agent-based Modeling and Simulation applications are used in many different areas like Biology, Medicine, Physics, Chemistry, Security, Social and Economic Modeling and range from minimalistic models to large scale decision support systems [29].\
...\
A frequently mentioned key objective when performing critical infrastructure modeling and simulation is to observe the dynamic effects caused by attacks, malfunctions, interruptions or disruptions of systems of critical infrastructure providers. The usage of simulation techniques enables analysts to improve their understanding about cascading and domino effects. [31] As the services provided by critical infrastructures are often unique, it can be observed that they are highly interconnected and interdependent amongst each other. That is the reason why the unavailability or improper functionality of one critical service can lead to far-reaching consequences. Besides the value for risk-assessment, modeling and simulation serves as information source for gaining new security knowledge about complex systems and can be further used to improve the planning of redundancies and incident response strategies as well as to facilitate the planning of exercises.\
...\
In order to get a holistic view on interdependencies between critical infrastructures, Rinaldi [30] demands six dimensions which should be considered: Type of failure (common cause, cascading, escalating), Infrastructure characteristics (organizational, operational, temporal, spatial), State of Operation (normal, repair/restoration, stressed/disrupted), Types of Interdependencies (physical, cyber, geographic, logical), Environment (economic, legal/regulatory, technical, social/political,
business, public policy, security, health/safety) and Coupling and Response Behavior (adaptive, loose/tight, inflexible, linear/complex). For a critical infrastructure simulation it is crucial to consider different impact categories. From the definitions introduced in Section I we derived the following impact areas caused by critical infrastructure failures: National economy, public order and social welfare, environment, national security/defense and health & safety [32], [3]. Failures concern a lot of different parties, private users, providers or other critical infrastructures. For the characterization of security requirements of a critical infrastructure provider we chose to implement well-known and widely used concepts and paradigms of security and dependability. One of the most popular approaches for defining security requirements is the CIA triad [33]. CIA stands for the three security goals confidentiality, integrity and availability defined by ISO 17799 respectively 27002 [34]:
* Confidentiality - ensuring that information is accessible only to those authorized to have access.
* Integrity - safeguarding the accuracy and completeness of information and processing.
* Availability - ensuring that authorized users have accessto information and associated assets when required. 

Although the CIA triad provides a solid foundation for the analysis of various threat scenarios, we decided to implement the concept of security and dependability as described by Avizienis et al. [35], [36], [37]. Dependability is described as ”. . . the ability to avoid service failures that are more frequent and more severe than [...] acceptable“ [37]. In addition to the adapted attributes confidentiality, integrity and availability, the authors [35] introduce the extended attributes reliability, safety and maintainability to seek security of systems.
* Confidentiality - is the non-occurrence of unauthorized disclosure of information.
* Integrity - is the non-occurrence of improper alterationsof information.
* Availability - ensuring the readiness for usage.
* Reliability - safeguarding the continuity of service.
* Safety - is the non-occurrence of catastrophic consequences on the environment.
* Maintainability - is the ability to undergo repairs and evolutions.
___

# Quotes from 6
___

**Stage 1.** CI description and scenario context (Section 2.2.1). A CI description provides a concrete context and concept of operation. This is the first level of scoping for the analysis task; the CI description gives the first indications of analysis boundaries. DSBM entities are identified and recorded.

**Stage 2.** Model development (Section 2.2.2). A model of the services (resources, inputs, outputs, system states) and the operational environment and system boundaries are developed, based on the CI description. Model boundary definitions are used at this stage to further restrict the scope of the analysis. Dependencies between the services are identified and the coupling points are defined: these refer on the one hand to the inputs and resources required by each of the services and on the other hand to the outputs that each of the services produces.

**Stage 3.** DSBM model development (Section 2.2.3). DSBMs are defined by selecting the right level of abstraction for the services: some of the services may be treated as black-boxes; in this case their representation in the DSBM will require no refinement in comparison with Stage 2. For those services, which are modelled in more detail one starts by defining explicitly their components and the assets including resort to using existing models of the underlying physical networks used by the services or use other formalisms, e.g. such as PVS [9]. A level of consistency is achieved between the service model and DSBM: the coupling points appear in both Views.

**Stage 4.** Initial dependency and interdependency identification (Section 2.2.4). While some of the service dependencies have already been identified and recorded in Stage 2 (via input/output/resource identification), at this stage the modeller looks for additional sources of dependence (e.g. common components/assets), which may make several services vulnerable to common faults or threats. These can be derived by examining the service-level model, taking into account other contextual information (e.g. scenarios, threat models, attacker profile). The captured dependencies are modelled as stochastic association between the services or components thereof. Each stochastic association is seen as a relationship between a parent and a child: the state of the parent affects the modelled behaviour of the child.

**Stage 5.** Probabilistic model development (Section 2.2.5). Since we are dealing with risk, we take the view that, given the state space formed by the modelled entities (MEs), a stochastic process must be constructed upon it that captures the unpredictable nature of the states of the MEs, their changes and the interactions between CIs over time. In this stage probabilistic models of the MEs are defined. These are state-machines, a well known formalism in software engineering, modelled after the formalism used in the Stochastic Activity Networks (SANs).

**Stage 6.** (optional) Adding deterministic models of behaviour (Section 2.2.6). At this stage the modeller may decide to extend the behaviour of the probabilistic model adding deterministic models of behaviour. Such a step may be useful when the modeller is seeking to extend the fidelity of the simulation beyond the standard mechanisms possible with a pure probabilistic model.

**Stage 7.** Exploratory interdependency analysis (Section 2.2.7). A Monte Carlo simulation [10] is used to quantify the impact of interdependencies on the behaviour of the system under study and draw more conclusions about the probability of interdependency-related risk. 
___

# Quotes 7
___

Cyber security of ICS has become a topic of active research (important contributions are summarised in the Related Research section). Its practical importance, the need for empirical studies and the difficulties with these, have been widely recognised. A common problem with cyber security research is that it concentrates on security incidents in the ICT/ICS, while the real impact of successful attacks is rarely quantified. As a result, quantitative risk assessment is difficult. While such an approach is, to some extent, justified in the ICT systems (for instance, how one assesses the impact of information theft is an open debate), with industrial systems the real impact of a cyber incident may be relatively easy to quantify. For instance, the impact of losing a generator in a power system as a result of a cyber-attack will vary between 0, in case other generators can provide additional power to compensate fully for the lost generator, to losses due to not supplying power to some consumers, in case the spare power generation capacity of the other generators in the network is insufficient to meet the current power demand.
___

# Quotes 8

___

The context within which PIA models are developed, and analysed, is defined by a scenario and related requirements. Here, the narrative aspect of a scenario is enormously important, as it provides the basis for asking questions and discovering interdependencies; typically, this is the starting point for the use of more formal models. 

Fig. 1 illustrates how one might start constructing, say, a service model, and identifying interdependencies between the services. Each of the services is likely to consist of various components. In Fig. 1 we show two services with their respective Information and Communications Technology (ICT), components, networks, and information assets. Some reasons why interdependencies may exist between services include: 
* Functional dependencies, i.e. a service consumes the output of another service as either input (e.g. oil is used as a raw material in a chemical plant and is subjected to transformation) or resource used (e.g. fuel for heating, or power for communication equipment); 
* Similar components, e.g. ICT components used in multiple services, via which common cause/mode failures may lead to simultaneous or related failures of the services (e.g. a virus may affect the computers running the same standard configuration of OS/applications used by different services providers); 
* Common environment. Stressful conditions in the environment are likely to increase the likelihood of failure or cause a failure of components in different services. Spatial dependencies are a typical example here, but one can easily envisage other forms too, e.g. services use the same cloud provider for their IT operation which will lead to simultaneous impact on both services if the cloud provider is stressed.
___

# Quotes 9
___

The proposed method for conducting quantitative analyses of interdependencies is based on the notions of performance indicators [11, 19], quality of service (QoS) [16] and dependence indices [40]. Since these terms are employed in different fields with various nuances, it is important to specify the meanings adopted in this research. The meanings mostly follow the definitions used in the information and communications technology (ICT) field. A performance indicator is a measurable quantity that an organization (public or private) adopts to quantify its success with respect to a specific goal or activity. In general, an evaluation of the performance of a system requires the definition and measurement of several performance indicators, each assessing a different characteristic. Managers and decision-makers often employ the set of performance indicators to enhance the performance of the system. In many cases, improving one performance indicator results in a decrease in another indicator. Thus, decisions are made by maximizing an appropriate objective function involving all the performance indicators. Quality of service is a broad term that refers to a quantitative index of the degree to which a service is appreciated by its users. The term is widely used in computer and communications networks, especially in telephone networks. The specific definition of quality of service is based on performance indicators relevant to the service of interest, typically various factors involving humans and cyber components (hardware and software). From the mathematical point of view, quality of service is simply an objective function based on user perspectives of a service. This research imposes the additional constraint of a positive and unitary objective function. A dependence index is a numerical measurement of the degree to which an activity (or service) depends on another activity (service), system or physical or human component. The term does not as yet have a uniform definition in the research literature on quantitative analyses of the interdependencies between the components of complex systems. However, in this research, a dependence index strictly refers to a quantitative estimate of dependence spanning the continuous interval [0,1].
___

1. [Discrete event simulation of wireless cellular networks](https://upcommons.upc.edu/bitstream/handle/2117/10201/discrete_event_simulation_of_wireless_cellular_networks.pdf)\
**MLA**: Zola, Enrica Valeria, Israel Martín Escalona, and Francisco Barceló Arroyo. "Discrete event simulation of wireless cellular networks." (2010): 263-284.\
**APA**: Zola, E. V., Martín Escalona, I., & Barceló Arroyo, F. (2010). Discrete event simulation of wireless cellular networks.

2. [Discrete event simulation with application to computer communication system performance](https://link.springer.com/content/pdf/10.1007/1-4020-8159-6_10.pdf)\
**MLA**: Szczerbicka, Helena, Kishor S. Trivedi, and Pawan K. Choudhary. "Discrete event simulation with application to computer communication systems performance." Information Technology. Springer, Boston, MA, 2004. 271-304.\
**APA**: Szczerbicka, H., Trivedi, K. S., & Choudhary, P. K. (2004). Discrete event simulation with application to computer communication systems performance. In Information Technology (pp. 271-304). Springer, Boston, MA.

3. [Stochastic reward net-based modeling approach for availability quantification of data center systems](https://www.intechopen.com/books/dependability-engineering/stochastic-reward-net-based-modeling-approach-for-availability-quantification-of-data-center-systems)\
**MLA**: Nguyen, Tuan Anh, et al. "Stochastic reward net-based modeling approach for availability quantification of data center systems." Dependability Engineering. IntechOpen, 2018.\
**APA**: Nguyen, T. A., Min, D., Choi, E., & García-Márquez, F. P. (2018). Stochastic reward net-based modeling approach for availability quantification of data center systems. In Dependability Engineering. IntechOpen.

4. [simmer: Discrete-Event Simulation for R](https://arxiv.org/pdf/1705.09746.pdf)\
**MLA**: Ucar, Inaki, Bart Smeets, and Arturo Azcorra. "simmer: Discrete-Event simulation for R." arXiv preprint arXiv:1705.09746 (2017).\
**APA**: Ucar, I., Smeets, B., & Azcorra, A. (2017). simmer: Discrete-Event simulation for R. arXiv preprint arXiv:1705.09746.

5. [A Generic Approach to Critical Infrastructure Modeling and Simulation](https://ieeexplore.ieee.org/abstract/document/6542537)\
**MLA**: Rybnicek, Marlies, et al. "A Generic Approach to Critical Infrastructure Modeling and Simulation." 2012 International Conference on Cyber Security. IEEE, 2012.\
**APA**: Rybnicek, M., Poisel, R., Ruzicka, M., & Tjoa, S. (2012, December). A Generic Approach to Critical Infrastructure Modeling and Simulation. In 2012 International Conference on Cyber Security (pp. 144-151). IEEE. 

6. [Preliminary Interdependency Analysis (PIA): Method and tool support](https://openaccess.city.ac.uk/id/eprint/3091/1/)\
**MLA**: Bloomfield, R. E., et al. "Preliminary interdependency analysis (PIA): Method and tool support." (2010).\
**APA**: Bloomfield, R. E., Chozos, N., Popov, P. T., Stankovic, V., Wright, D., & Howell-Morris, R. (2010). Preliminary interdependency analysis (PIA): Method and tool support.

7. [Model-based evaluation of the resilience of critical infrastructures under cyber attacks](https://openaccess.city.ac.uk/id/eprint/4364/1/)\
**MLA**: Netkachov, Oleksandr, Peter Popov, and Kizito Salako. "Model-based evaluation of the resilience of critical infrastructures under cyber attacks." International Conference on Critical Information Infrastructures Security. Springer, Cham, 2014.\
**APA**: Netkachov, O., Popov, P., & Salako, K. (2014, October). Model-based evaluation of the resilience of critical infrastructures under cyber attacks. In International Conference on Critical Information Infrastructures Security (pp. 231-243). Springer, Cham.

8. [Preliminary interdependency analysis: An approach to support critical-infrastructure risk-assessment](https://www.sciencedirect.com/science/article/pii/S0951832017305963)\
**MLA**: Bloomfield, Robin E., et al. "Preliminary interdependency analysis: An approach to support critical-infrastructure risk-assessment." Reliability Engineering & System Safety 167 (2017): 198-217.\
**APA**: Bloomfield, R. E., Popov, P., Salako, K., Stankovic, V., & Wright, D. (2017). Preliminary interdependency analysis: An approach to support critical-infrastructure risk-assessment. Reliability Engineering & System Safety, 167, 198-217.


9. [A methodology for modeling and measuring interdependencies of information and communications systems used for public administration and eGovernment services](https://www.academia.edu/download/57020978/nicola2016.pdf)\
**MLA**: De Nicola, Antonio, et al. "A methodology for modeling and measuring interdependencies of information and communications systems used for public administration and eGovernment services." International Journal of Critical Infrastructure Protection 14 (2016): 18-27.\
**APA**: De Nicola, A., Villani, M. L., Brugnoli, M. C., & D'Agostino, G. (2016). A methodology for modeling and measuring interdependencies of information and communications systems used for public administration and eGovernment services. International Journal of Critical Infrastructure Protection, 14, 18-27.


