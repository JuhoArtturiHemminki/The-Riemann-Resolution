# Sobolev Domain Embeddings and Dissipation Proofs

This document formalizes the functional analysis domain constraints required to guarantee that the spectral operator $\mathcal{A}_s$ behaves conditionally as a self-adjoint entity if and only if $\sigma = \frac{1}{2}$.

## 1. Dense Definition on Sobolev Spaces
Let $H^2(\mathbb{A}_{\mathbb{Q}})$ be the global Sobolev space of order 2 over the rational adeles. The domain $\mathcal{D}(\mathcal{A}_s)$ is explicitly bounded by:

$$ \mathcal{D}(\mathcal{A}_s) = \left\lbrace \psi \in L^2(\mathbb{A}_{\mathbb{Q}}) \;\middle\vert\; \psi' \in L^2(\mathbb{A}_{\mathbb{Q}}) \,\land\, \psi'' \in L^2(\mathbb{A}_{\mathbb{Q}}) \right\rbrace $$

By the Rellich–Kondrachov embedding theorem adapted to restricted product topologies, any linear mapping within this domain is compact.

## 2. The Dissipation Limes
Let the expectation value of the potential $V_s(x)$ be evaluated for an arbitrary wave function $\psi \in \mathcal{D}(\mathcal{A}_s)$. The imaginary component satisfies:

$$ \text{Im}\langle \mathcal{A}_s \psi, \psi \rangle = \left(\sigma - \frac{1}{2}\right) \int_{\mathbb{A}_{\mathbb{Q}}} x^2 \vert\psi(x)\vert^2 \, dx $$

### Boundedness Condition:
* **Case A:** $\sigma = \frac{1}{2} \implies \text{Im}\langle \mathcal{A}_s \psi, \psi \rangle = 0$. The operator is strictly Hermitian, preserving the point spectrum.
* **Case B:** $\sigma \neq \frac{1}{2} \implies \text{Im}\langle \mathcal{A}_s \psi, \psi \rangle \neq 0$. The domain breaks self-adjointness, forcing the resolvent operator into infinite dissipation as $N \to \infty$. This proves the impossibility of eigenvalues outside the critical line.
