
## 1. Introduction to Transportation Planning

- **Definition:** A process of looking ahead and setting a course of action to satisfy future transportation needs.
    
- **Core Question:** How to allocate resources effectively?
    
      
    - Infrastructure projects take a long time to build and require planning well in advance.
        
    - Addresses critical questions: _Who, What, Where, When, Why, How_.

- **Planning Types:**
    
      
    - **Short- or Medium-Term Planning:** Less complex; focuses on optimal operation of existing facilities under budget constraints.

    - **Long-Term (Strategic) Planning:** Highly complex; involves large, extensive construction programs requiring a **system approach** instead of a single-project philosophy.

- **System Approach & System Engineering:** Tackled by an interdisciplinary team (transportation engineers, urban planners, economists, environmentalists, demographers) rather than a single discipline.

- **Basic Elements of Long-Term Planning:**
    
      
    1. Forecast system demand (economic, social, environmental changes).
        
          
        
    2. Evaluate options based on benefits/disbenefits to three groups:
        
          
        - **Operators:** Operating costs, revenues.
            
              
            
        - **Users:** Monetary costs, travel time, safety, comfort.
            
              
            
        - **Non-users:** Air/water pollution, noise, safety, economic effects, land use changes.
            
              
            

## 2. Regional Transportation Planning & Land Use Interaction

- **Metropolitan Planning Organizations (MPOs):** Responsible for developing Regional Transportation Plans (RTP) using a **Continuing, Cooperative, and Comprehensive (3-C)** planning process.
    
      
    
- **Cyclic Interaction Between Transportation and Land Use:**
    
      
    - _Land Use $\rightarrow$ Transportation:_ Changed land use (more residents/employees) brings more passenger travel demand and commercial/industrial areas increase freight demand.
        
          
        
    - _Transportation $\rightarrow$ Land Use:_ Added transportation facilities increase accessibility, which raises land value and potential, leading to further land use changes.
        
          
        

## 3. Travel Demand Models (The 4-Step Model)

- **Travel Demand:** Travel for activities at different places.
    
      
    
- **Trip:** One-way movement from an origin to a destination.
    
      
    
- **The Four-Step Travel Demand Model Pipeline:**
    
      
    1. **Trip Generation:** _How many trips?_ Estimates productions and attractions.
        
          
        
    2. **Trip Distribution:** _Where are they going?_ Connects origins to destinations.
        
          
        
    3. **Mode Split:** _By what mode?_ (e.g., auto, transit, walk)
        
          
        
    4. **Traffic Assignment:** _What path to take?_ Assigns trips to the physical network.
        
          
        

## 4. Data Inputs

- **Travel Survey:** Records individual journeys (origin, destination, time, purpose, socio-economic attributes).
    
      
    
- **Socio-Economic Data (SED):** Household size, age, workers, income, employment by industry, school enrollment.
    
      
    
- **Network Data:** Highway/transit networks, vehicle counts, posted speeds, parking costs, auto operating costs, value of time.
    
      
    

## 5. Step 1: Trip Generation

- **Traffic Analysis Zones (TAZ):** Small sub-areas used to aggregate and represent origins and destinations instead of individual addresses. Uses TAZ centroids connected to the highway network via **centroid connectors** (pseudo-links).
    
      
    
- **Trip Purposes:** Differentiated to capture varying temporal demands (Home-Based Work [HBW], Home-Based School [HBSc], Home-Based Shopping [HBSh], Home-Based Recreation [HBR], Home-Based Other [HBO], Non-Home-Based [NHB]).
    
      
    
- **Trip Production Model:**
    
      
    - Estimated primarily at the **household level** (easier data collection, correlates with income and size).
        
          
        
    - Calculated via cross-classification (Trip Production = $\sum r_i \times f_i$, where $r_i$ = trip rate and $f_i$ = household frequency).
        
          
        
- **Trip Attraction Model:**
    
      
    - Estimated using land use data, typically employment types (retail, service, office) and school enrollment.
        
          
        
    - Modeled via regression: $A = r_1 E_1 + r_2 E_2 + \dots$
        
          
        
- **Trip Balance Process:** Total regional productions must equal total attractions. Scale factors ($P/A$ ratios) are applied to adjust trip generation outputs if they do not initially balance.
    
      
    

## 6. Step 2: Trip Distribution & Network Skims

- **Highway Networks & Graphs:** Modeled as nodes and links with attributes like distance and travel time.
    
      
    
- **Shortest Path & Skim Matrix:**
    
      
    - **Dijkstra’s Algorithm:** Used to find the shortest path tree from a TAZ centroid to all other nodes.
        
          
        
    - **Skim Matrix:** A square matrix storing accumulated non-negative link attributes (travel time, distance, tolls) along shortest paths between all TAZ pairs.
        
          
        
- **Gravity Model:**
    
      
    - Analogous to Newton's law of universal gravitation ($T_{ij} \propto P_i A_j f(t_{ij})$).
        
          
        
    - **Singly-Constrained (Production-Constrained) Gravity Model:**
        
          
        
        $$T_{ij} = \frac{P_i A_j F_{ij}}{\sum_{k=1}^{Z} A_k F_{ik}}$$
        
        - Where $F_{ij} = \exp(-\beta \cdot t_{ij})$ is the **friction factor** (a decreasing function of travel time).
            
              
            
    - **Doubly-Constrained Gravity Model:**
        
          
        - Uses the **Iterative Proportional Fitting (IPF)** algorithm when both row sums (productions) and column sums (attractions) must simultaneously match target controls. Alternately scales rows to match $P_i$ and columns to match $A_j$ until convergence.