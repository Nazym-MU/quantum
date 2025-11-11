# Uncertainty Relations Schwarz Inequality Derivation

Derives ΔA·ΔB ≥ |⟨C⟩|/2 when [Â, B̂] = iĈ using Cauchy-Schwarz inequality.

## Starting Point: Schwarz Inequality
$$(⟨α|α⟩)(⟨β|β⟩) ≥ |⟨α|β⟩|²$$

## Step 1: Define States
$$|α⟩ = (Â - ⟨A⟩)|ψ⟩$$
$$|β⟩ = (B̂ - ⟨B⟩)|ψ⟩$$

Then:
$$⟨α|α⟩ = ⟨ψ|(Â - ⟨A⟩)²|ψ⟩ = (ΔA)²$$
$$⟨β|β⟩ = (ΔB)²$$

## Step 2: Evaluate ⟨α|β⟩
$$⟨α|β⟩ = ⟨ψ|(Â - ⟨A⟩)(B̂ - ⟨B⟩)|ψ⟩$$

Split any operator Ô into Hermitian parts:
$$Ô = \frac{Ô + Ô†}{2} + \frac{Ô - Ô†}{2}$$

Define:
- F̂ = Ô + Ô† (Hermitian)
- Ĝ = -i(Ô - Ô†) (Hermitian)

For Ô = (Â - ⟨A⟩)(B̂ - ⟨B⟩):
$$Ô - Ô† = [Â, B̂] = iĈ$$

Therefore Ĝ = Ĉ and:
$$⟨α|β⟩ = \frac{⟨F⟩}{2} + \frac{i⟨C⟩}{2}$$

## Step 3: Use Triangle Inequality
$$|⟨α|β⟩|² = \left|\frac{⟨F⟩}{2}\right|² + \left|\frac{⟨C⟩}{2}\right|²$$

Since ⟨F⟩ and ⟨C⟩ are real (Hermitian operators):
$$|⟨α|β⟩|² = \frac{⟨F⟩²}{4} + \frac{⟨C⟩²}{4} ≥ \frac{⟨C⟩²}{4}$$

**Key step:** Drop positive term ⟨F⟩²/4 ≥ 0 to get inequality.

## Step 4: Apply Schwarz Inequality
$$(ΔA)²(ΔB)² ≥ |⟨α|β⟩|² ≥ \frac{⟨C⟩²}{4}$$

Taking square root:
$$\boxed{\Delta A \cdot \Delta B ≥ \frac{|\langle C \rangle|}{2}}$$

## See
- [[General Uncertainty Relation from Commutators]]