# TL;DR

The [RustCI/CommitID](https://community-ci.openruyi.cn/rustci/job/RustCI/job/CommitID/) job is the entry point of the Rustci pipeline. It can accept a **commit SHA-1 hash**  or a GitHub PR ID from the
[rust-lang/rust](https://github.com/rust-lang/rust) repository (both are optional). Upon triggering, it invokes the [RustCI/check](https://community-ci.openruyi.cn/rustci/job/RustCI/job/RustCheck/)
job, which subsequently distributes the parallel execution of check and test jobs.


# goal
[Rustci](https://community-ci.openruyi.cn/rustci/) aims to provide stable and reliable riscv64 hardware for the Rust community, with the goal of elevating Rust's riscv64 support to Tier 1 status.

# Current Status
Rustci is currently under active development. As you may have observed, certain tests are currently failing on riscv64. We are planning to establish a test cases baseline and implementing automated cron
monitoring to detect [regressions](https://github.com/rust-lang/gccjit.rs/pull/64) on the riscv64 as early as possible.

During this phase, we welcome your feedback and aim to help you test your rustc patches on riscv64 hardware. Simultaneously, we are awaiting guidance
from the Rust T-infra team on integrating this system into the official CI pipeline if [this is allowed](https://rust-lang.zulipchat.com/#narrow/channel/242791-t-infra/topic/We're.20eager.20to.20provide.20the.20community.20with.20RISC-V.20CI.20infrastr/near/560991877).


# issues
If you have any issue about this pleaase open one [issue](https://github.com/OERV-RVCI/rustci4rv/issues/new) to report it.

We currently grant anonymous users read-only access.