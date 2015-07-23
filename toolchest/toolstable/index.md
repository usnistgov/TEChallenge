---
title: Table of Tools
layout: page
---
#TE Challenge Modelling and simulation tools and co-simulation environments

### Table of Contents
  * **[Non-commercial Simulation Tools](#Non-commercial-Tools)**
  * **[Commercial Simulation Tools](#Commercial-Tools)**
  * **[Co-simulation Platforms](#Co-simulation)**

<a name="Non-commercial-Tools"></a> 

-------------------------------------------------------------

##Non-commercial Simulation Tools

| **Non-commercial tools**     | **Function/uses**     |
|------------------------------|-----------------------|
| [Gridlab-D](http://www.gridlabd.org/) | Retail markets, physical constraints, end use load models for distribution systems; slow moving dynamics over time. Solves equilibrium type problems; agent based.                            
|BSD license| * Distribution system modeling tool developed by PNNL.|
|on Sourceforge| * Market simulation environment.|
||* Power flow analysis.|
||* Future power initiative on bulk power side.|
||* Extendable environment, can submit modification requests (or submit code extensions for review)|
||* Limitation: Only real power and not reactive power.|
||* Logical time, time scale down to 1-sec, maybe federate in a tool that can handle faster time scales.|
||* Users: open source, users group, engineer oriented, command line interface, 3<sup>rd</sup> party GUIs|
||* Economics: Wholesale market model, economic dispatch model, models retail and wholesale interactions, understands LMP|
||* Features: can work with other modeling packages: wholesale market, GOSS, FNCS (integration)|
||* Has been integrated with EnergyPlus (building energy modeling tool)|
|
| [openDSS](http://smartgrid.epri.com/SimulationTool.aspx)| EPRI distribution system power simulation|
|BSD license| * capable of faster system dynamic modeling|
|on Sourceforge| * Open source with strong user group|
||* Originally a teaching tool, has grown to be a professional quality tool | 
||* There is beginning to be a migration away from Aspen/Cape to this platform (good alternative)|
||* Includes both physics and economics (earlier tools are just physics)|
||* Comparison to GridlabD. Different system architecture. SS analysis, not transient.|
|
| [Modelica](https://www.modelica.org/) (open source)| Modelica is a non-proprietary, object-oriented, equation based language to conveniently model complex physical systems containing, e.g., mechanical, electrical, electronic, hydraulic, thermal, control, electric power or process-oriented subcomponents.      Multi-physics simulation package; multi domain includes power system simulation library; equation based simulator; simulation language; there are public and private tools -- [OpenModelica](http://alternativeto.net/software/openmodelica/) is open source; [Dymola](http://www.3ds.com/products-services/catia/capabilities/modelica-systems-simulation-info/dymola) is a proprietary tool.|
|
| [AMES](http://www2.econ.iastate.edu/tesfatsi/AMESMarketHome.htm) (open source)| Iowa State wholesale power market simulator; 
||* agent based framework
||* Economic dispatch
||* Unit commitment
||* Steady state analysis
||* Example use: RTO environment (Cal ISO)
|
| [EnergyPlus](http://apps1.eere.energy.gov/buildings/energyplus/) | DOE Physics based building simulation package   
|
| [NS-3](https://www.nsnam.org/) GNU GPLv2 license| NS-3 is a discrete-event network simulator for Internet systems, targeted primarily for research and educational use. Can be coupled with GridLab-D.
||* can work with bidding concepts (accepting, managing)
||* can communicate market clearing price   can simulate demand response
|
| ORNL [THYME](http://web.ornl.gov/~1qn/thyme/docs/)| Simulation tool for studying the interaction of controls, communications, and electro-mechanical dynamics in a power system. THYME is C++ library for building simulators that integrate its modules for power system dynamics with existing simulators for communication networks (e.g., NS/2 and OMNET++), discrete control systems, and discrete event simulation packages in general.
|
| U Wisc [TRNSYS](http://sel.me.wisc.edu/trnsys/)   | Building simulation. TRNSYS is a transient systems simulation program with a modular structure. The TRNSYS library includes components found in thermal and electrical energy systems, and handles input of weather data or other time-dependent forcing functions and output of simulation results.
|
| NIST [HVACSIM+](http://fire.nist.gov/bfrlpubs/build08/PDF/b08030.pdf)| HVAC dynamic simulation (NIST)
|
| DOE [SPIDERS](http://energy.sandia.gov/infrastructure-security/energy_surety/spiders/)| Microgrid simulation
||* FORTRAN, converted to more modern languages (C, JAVA)
||* Originally diesel-fuel focused but has been expanded and adapted
||* used to support a balance of supply and demand at military facilities
||* Intended to model/manage load/generation for on-base microgrids
|
| [OMF](http://www.nreca.coop/what-we-do/bts/smart-grid-demonstration-project/open-modeling-framework/) | Open Modeling Framework provides a wrapper around Gridlab-D with library and import support. OMF development is led by the NRECA Cooperative Research Network.  OMF enables utilities to evaluate smart grid components using real-world data prior to purchase. OMF supports co-op investment decision-making by modeling the cost and benefits, incorporating engineering, weather, financial and other data specific to the co-op. OMF provides common data models, configuration management tools, run execution and visualization capabilities for use with multiple models, including the PNNL’s Gridlab-D and the NREL’s System Advisor Model.

<a name="Commercial-Tools"></a> 

------------------------

##Commercial Simulation Tools

| **Commercial Tools** | **Function/Uses** |
|----------------------|-------------------|
| [OPAL-RT](http://www.opal-rt.com/electrical-system-simulation-overview)    | Hardware in the loop simulator. Multidomain. OPAL-RT provides real-time digital simulators and control prototyping systems for power grids and power electronics.
|
| [RTDS ](https://www.rtds.com/)  | Realtime digital power system simulator; hardware in the loop; Protection Systems Testing; Control Systems Testing; PMU Studies; Smart Grid and Distributed Generation.
|
| [Matlab](http://www.mathworks.com/products/matlab/) tools| Language for technical computing; integrates computation, visualization, and programming in an environment where problems and solutions are expressed in familiar mathematical notation.
||* Simulink—Data flow graphical programming language tool for modeling, simulating and analyzing multi-domain dynamic systems.
||* MATpower—package of Matlab M-files for solving power flow and optimal power flow problems. Can use for transmission-level bulk market.
||* PowerSim—power system simulator-Mathworks tool
|
| [ETAP](http://etap.com/) | Electrical Power system design and operation simulation. ETAP offers a suite of fully integrated electrical engineering software solutions:
||* Power system design and analysis
||* Real-time power management system
||* Smart grid and microgrid solution
||* power flow and load shedding
|
| [Plexos](http://energyexemplar.com/software/plexos-desktop-edition/)   | PLEXOS® Integrated Energy Model: Simulation software for energy market analysis. PLEXOS meets the demands of energy market participants, system planners, investors, regulators, consultants and analysts, integrating electric, gas, water and heat production, transportation and demand over simulated timeframes from minutes to 10’s of years
|
| [Promod](http://www.ventyx.com/~/media/files/brochures/promod_data_sheet.ashx)   | Generator and Portfolio Modeling System with Nodal LMP, Forecasting & Transmission Analysis. Promod IV is an Electric Market Simulation solution, incorporating extensive details in generating unit operating characteristics, transmission grid topology and constraints, and market system operations.
|
| [PSS/E](http://www.energy.siemens.com/us/en/services/power-transmission-distribution/power-technologies-international/) and [PSLF](http://site.ge-energy.com/prod_serv/products/utility_software/en/ge_pslf/index.htm) | PSLF: GE Positive Sequence Load Flow Software (PSLF) is a full-scale program designed to perform load flow, dynamic simulation, and short circuit analysis. Typically used by power system engineers for simulating the transfer of large blocks of power across a transmission grid.  PSS/E: The Power System Simulator for Engineering or PSS/E, essentially has the same system capability as PSLF a software program. This package is typically used by electrical transmission planners performing load flow, dynamic simulation, and short circuit analysis for obtaining a reliable power system    Example use: power plant and windfarm siting, relay coordination for protection
|
| GE [MAPS](http://www.geenergyconsulting.com/practice-area/software-products/maps)  | Modeling of the economic operation of the power system
|
| [UPLAN](http://www.energyonline.com/) | * A Complete System for Integrated Market Simulation, Price Forecasting, Optimal Power Flow, Asset Valuation and Risk Management
||* The Electricity Competition Analysis and Marketing System
||* Production cost model for the power system.
|
| ABB [GridView](https://library.e.abb.com/public/581366a0c212c93ac1256fda00488562/Gridview%20Brochure.pdf)    | Energy markets and analysis simulation tool
|
| [Aspen](http://www.aspeninc.com/web/index.html), [Cape](http://www.electrocon.com/tslink.php)  | ASPEN--Suite of tools for grid modeling. Example use: model switches & the effect of switching (large loads) CAPE-TS Link™ is a simulation tool that gives electric power grid engineers the ability to design and evaluate the fast, wide-area control needed to avoid cascading outages and blackouts.
|
| DIgSILENT [PowerFactory](http://www.digsilent.com/)   | Integrated power systems modelling and analysis package. Good for balancing/dynamic issues. Emerging market grid simulators.
|
| [HOMER](http://www.homerenergy.com/software.html)  | HOMER's optimization and sensitivity analysis algorithms allow you to evaluate the economic and technical feasibility of a large number of microgrid technology options. Residential scale up to 1MW (neighborhood scale)    Some capability to model energy usage in the home. Models transactional energy choices. Life cycle cost analysis.
|
| [PowerWorld](http://www.powerworld.com/)| Tools for transmission planners, power marketers, system operators; mainly transmission level simulations.|

<a name="Co-simulation"></a> 

----------------------------------------

##Co-simulation Platforms

| **Platform**      | **Notes**        |
|-------------------|------------------|
| [HLA](http://en.wikipedia.org/wiki/High-level_architecture_%28simulation%29 ) | High-Level Architecture, IEEE Standard 1516. Semantics based, time based, risk based, geographically based ontologies.  Can integrate data from multiple sources into a more cohesive whole. Can add such things as weather and economics.
|
| [FNCS](https://github.com/GridOPTICS/FNCS-gridlab-d ) | PNNL Framework for network co-simulation; tool based on HLA standards. FNCS designed to enable co-simulation with GridlabD, where GridlabD is specific to power domain. [Fuller PPT from workshop](http://www.nist.gov/el/building_environment/mechsys/upload/PNNL-Simulation-Jason-Fuller.pdf )
|
| [C2WT](https://wiki.isis.vanderbilt.edu/OpenC2WT/index.php/Main_Page ) | Model and simulation integration layer above HLA. [Vanderbilt C2](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.156.7106&rep=rep1&type=pdf ) has general purpose background aimed at integrating different domains. See also the [Sztipanovits presentation](http://www.nist.gov/el/building_environment/mechsys/upload/Vanderbilt-C2WT-Sztipanovits.pdf )from the workshop. 
|
| [FMI/FMU](http://en.wikipedia.org/wiki/Functional_Mock-up_Interface ) | Functional mockup interface and implementation
|
| [DIS](http://en.wikipedia.org/wiki/Discrete_event_simulation ) | DOD standard discrete event simulator IEEE 1278
|
| [CRex](http://energy.gov/sites/prod/files/2015/04/f22/SmartCloud%20-%20Hunt.pdf ) | Commercial semantic historian product for IoT applications, SmartCloud, Inc.|


