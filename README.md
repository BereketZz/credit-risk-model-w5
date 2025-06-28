# credit-risk-model-w5
<section>
  <h2>Credit Scoring Business Understanding</h2>

  <h3>1. Influence of Basel II on Model Interpretability and Documentation</h3>
  <p>
    The Basel II Accord mandates that financial institutions measure and manage credit risk more rigorously by integrating internal risk models into their capital adequacy calculations. This regulation places a premium on 
    <strong>model transparency, interpretability, and documentation</strong>, as regulators require clear justifications for how risk estimates are derived.
    Consequently, credit scoring models must not only perform well but also be 
    <strong>auditable and explainable</strong>, reinforcing the need for well-structured models where each feature’s contribution to the risk score is understandable by both business users and regulatory bodies.
  </p>

  <h3>2. The Need for a Proxy Variable in the Absence of a Default Label</h3>
  <p>
    In many credit risk datasets, a direct "default" outcome may be missing or inconsistently defined. To proceed with modeling, it's necessary to create a 
    <strong>proxy variable</strong>—for example, labeling customers as "bad" if they are 90+ days past due within 12 months. 
    This enables supervised learning but introduces 
    <strong>risk of label misalignment</strong>. 
    If the proxy does not accurately capture true default behavior, predictions may be skewed, leading to 
    <strong>inappropriate credit decisions</strong>, regulatory scrutiny, or financial losses from misclassified risk.
  </p>

  <h3>3. Trade-offs Between Simple and Complex Models</h3>
  <p>
    Simple models like 
    <strong>Logistic Regression with Weight of Evidence (WoE)</strong> offer high interpretability, stable performance, and compliance with regulatory expectations. 
    These models allow for easy validation and insight into the drivers of risk. However, they may lack the flexibility to capture complex nonlinear interactions in the data.
    On the other hand, 
    <strong>complex models like Gradient Boosting</strong> can offer higher predictive accuracy but at the cost of reduced transparency and greater difficulty in explaining decisions. 
    In regulated environments, this introduces challenges in model governance, explainability, and justification, which can limit their practical deployability despite better performance.
  </p>
</section>
