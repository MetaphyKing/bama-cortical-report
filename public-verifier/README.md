# BAMA v3.1 Read-Only Public Verifier SDK (`bama_public_verifier_sdk.zip`)

**Author:** Logan Smith · Metaphy LLC  
**Intellectual Property Status:** U.S. Provisional Patent Application Filed / Patent Pending (`35 U.S.C. § 111(b)`).  
**Companion Paper:** *"How BAMA Elevates Local AI to Frontier Performance — Cortical Amplification"* (Version 3.1, October 2026)

---

## What Is Included in This Public Verification Package?

To enable independent peer reviewers, MLSys artifact evaluators, and enterprise partners to verify BAMA's binary cell geometry, mathematical invariants, and empirical benchmark receipts **without exposing Metaphy LLC's proprietary offline $W_1$–$W_4$ cognitive compiler or Dual-Cap B.I.F.R.O.S.T. ingestion engine**, this SDK ships the pre-compiled binary `.bin` cartridges alongside a standalone, read-only Python verifier:

1. **`bama_72_kernel_prime_arena.bin` (`18,432 Bytes` = `72 x 256-Byte ZDC-QEGG Cells`):**
   - SHA-256: `d35fffdc410bb6a1d7ae95976ae28c36133230dbb4fdaa534b50a36fc7ad7b6b`
2. **`bama_80_multimodal_collective_qegg.bin` (`20,480 Bytes` = `80 x 256-Byte ZDC-QEGG Cells`):**
   - SHA-256: `88ee90dc9ee95eb2e92c39130a8b0ac08d0197598aabe4d00fdebe954b9f9cab`
3. **`BAMA_BLIND_PRIMED_72KERNEL_BENCHMARK.json` & `BAMA_HONEST_UNPRIMED_INDUSTRY_BENCHMARK.json`:**
   - Complete machine-verifiable receipts for the 5-task (`15` deterministic sub-assertion: `1+3+3+4+4`) evaluation across Tiers `T1–T5b`.
4. **`verify_bama_public_cartridge.py`:**
   - Standalone read-only verification script (requires only Python 3.10+ and `numpy`).

---

## Quick Start (`< 1 Second`)

```bash
python verify_bama_public_cartridge.py
```

### What `verify_bama_public_cartridge.py` Verifies:
- **Gate 1:** Byte-exact `256-byte` (`4 CPU cache lines`) cell alignment, SHA-256 digests, `QEG5` magic headers, `dtype_code == 10` (`SUBSTRATE_PHI_POWER`), and `INV-10` recursion bounds (`fractal_depth <= 6`, `unfold_ops_budget <= 4096`).
- **Gate 2:** Zero-Decompression $\mathbb{Z}[\varphi]$ Two-Accumulator inner product ($\langle \mathbf{q}, \hat{\mathbf{w}} \rangle = s \cdot (A_{\text{unit}} + \varphi A_\varphi)$) with `0 Bytes` of Float32 decompression buffer allocation (`12.0x` compression over Float32).
- **Gate 3:** GAAMA 2-Hop Personalized PageRank with degree-threshold hub dampening ($\text{damp}(d) = \min(1.0, \theta/d)$, $\alpha=0.15, \theta=50$), verifying `TARGET_SPEC = 0.180625`, undamped `TARGET_HUB = 0.003577`, damped `TARGET_HUB = 0.001771` (`-50.50%` at $d=101$), and the `102.01x` target-to-hub specificity ratio.
- **Gate 4:** Audit of the unprimed (`T1–T5a`) and BAMA-primed (`T3b–T5b`) 5-task benchmark receipts.
