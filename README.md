Supply Chain Optimization — Linear Programming

A linear programming model designed to minimize shipping costs in a multi-supplier supply chain. The model determines the optimal allocation of products across suppliers while satisfying stock demand requirements and supplier availability constraints.

Result: Achieved a minimum total shipping cost of £279.00

📊 Dataset

Source: Sales company supply chain data

Key Variables:

SKU: Product identifiers

Stock levels: Required quantity per product

Availability: Maximum units each supplier can provide

Shipping costs: Cost per unit from each supplier

Supplier name: Supplier identifiers

Size: Multiple SKUs across 3 suppliers

⚙️ Methodology
1. Data Preprocessing

Created complete SKU–supplier combination matrix

Handled missing shipping costs

Scaled stock levels to match total supplier availability

2. Model Formulation

Decision Variables: Quantity to ship from each supplier per SKU

Objective Function: Minimize total shipping cost

Constraints:

Meet required stock demand

Respect supplier capacity limits

3. Optimization

Implemented using PuLP (Python linear programming library)

Solved with LP solver to compute the optimal allocation

🚧 Challenges

Data Completeness: Missing SKU–supplier combinations required generating a complete pairing matrix

Constraint Balance: Initial demand exceeded supply, requiring proportional scaling

Feasibility: Adjusted model to ensure total demand aligned with supplier availability

✅ Key Features

Automated optimal allocation of products across suppliers

Minimizes costs while satisfying real-world operational constraints

Scalable to any number of products and suppliers

Outputs clear shipment allocation per supplier

📌 Recommendations

Procurement Strategy: Use outputs for weekly/monthly procurement planning to maintain cost efficiency

Supplier Negotiations: Leverage high-volume allocations to negotiate better shipping rates

Dynamic Updates: Integrate with real-time inventory data for continuous optimization

Capacity Planning: Monitor supplier availability patterns to anticipate bottlenecks
