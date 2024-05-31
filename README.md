# Transhipment-with-fixed-costs-optimization-model

Pulp & Paper Ltd. produces cardboard at 3 mills in Finland, Sweden, and Belgium. From the mills, the cardboard is transported to 4 warehouses located in Finland, Lithuania, Czech Republic, and the UK, and then the sheeted cardboard to 13 customer areas.

The Sales & Marketing department has just released its demand estimates for the following month and unfortunately, the total demand exceeds the total production capacity. The mills have informed Sales & operations of the extra capacity they could provide for the following month and also provided estimates on the cost of making use of this extra capacity.

The Advanced Analytics team has formulated a MILP model that extends the transshipment model you are familiar with to also optimize decisions on the use of the extra capacity. The model is as follows:

Indexes:
𝑀={0,1,2}: Mills  
𝑊={0,…,3}: Warehouses 
𝐶={0,…,12}: Customer areas

Parameters:
𝑑_𝑗: demand in customer area 𝑗  
𝑝_𝑖: production capacity at mill  𝑖  
𝑒_𝑖: extra production capacity at mill  𝑖  
𝑐_𝑖𝑘^𝑎: tranportation costs per ton from mill 𝑖 to warehouse 𝑘   
𝑐_𝑘𝑗^𝑏: tranportation costs per ton from warehouse 𝑘 customer area 𝑗
𝑐_𝑖^𝑒:  cost of using the extra production capacity at mill  𝑖  

Decision variables:
𝑥_𝑖𝑘: Tons transported from mill 𝑖 to warehouse 𝑘   
𝑦_𝑘𝑗: Tons transported from warehouse 𝑘 customer area 𝑗
𝑧_𝑖: Use extra capacity at mill  𝑖   

# Objective: 

Create an run an optimization model to minimize the cost throughout the entire logistic process.



