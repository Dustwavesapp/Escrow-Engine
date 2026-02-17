Escrow Engine
Dispute-aware escrow. Third-party arbiter resolution, partial release, expiry refund, fee splitting.
Implement an Escrow Engine with the following lifecycle:

create_escrow

Define depositor, beneficiary, arbiter, amount, expiry timestamp, fee structure.

release_funds

Full or partial release initiated by mutual consent or arbiter decision.

raise_dispute

Lock escrow state and restrict unilateral actions.

resolve_dispute

Arbiter allocates funds (full or partial) according to adjudication.

expire_escrow

Automatically refund funds to depositor if no resolution occurs before expiry.

Security requirements:

Idempotent state transitions.

Strict authority checks.

Reentrancy protection.

Overflow/underflow guards.

Deterministic and auditable balance tracking.

The implementation must follow best practices for secure contract design and be suitable for real-world commercial transactions.
