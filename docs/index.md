## rlxos GNU/Linux

rlxos is an independent initiative dedicated to creating a **secure, reliable, and high-performance operating system** based on the Linux kernel. Our vision is to bring **Android-like security** and workflow to desktop systems, while maintaining full functionality and customization options for users.

At the heart of rlxos is its **sysroot-managed immutable root filesystem**, powered by **libostree**, which introduces a suite of advanced features designed to enhance system integrity and performance:

- **Atomic Updates:** Updates are applied in a fully transactional manner, ensuring that the system is never left in an incomplete or unstable state.
- **Seamless Version Rollback:** Easily revert to a previous system version in case of issues with a new update, minimizing downtime and troubleshooting efforts.
- **Modular Software Expansion via Extensions:** Software can be installed as extensions, leaving the core system untouched, offering flexibility without sacrificing stability.
- **Delta Updates for Efficient Bandwidth Usage:** Only the differences between system versions are downloaded, significantly reducing bandwidth consumption during updates.

### Immutable Root Filesystem

An **immutable root filesystem** refers to a system design where the root filesystem is **read-only**, protecting it from standard modifications. This design is key to enhancing system security and stability, as it prevents unwanted changes to core components. In rlxos, this concept is realized through **libostree**, which also enables features such as atomic updates and rollbacks.

#### Benefits:
- **Enhanced System Integrity:** The read-only nature of the filesystem safeguards against corruption and accidental modifications.
- **Improved Security:** Unauthorized changes to critical system files are nearly impossible, significantly bolstering security.
- **Predictable and Consistent Environment:** A stable, consistent system state benefits users and developers by reducing unexpected issues and enhancing reliability.

#### Drawbacks:
- **Reduced Customization Flexibility:** The inability to modify core system files may be limiting for users who prefer full control over their system.

### Why rlxos?

- **Security-Driven Design:** rlxos is built around a security-first philosophy, using an immutable root filesystem to protect the system from unintended changes.
- **Reliable and Consistent Updates:** Atomic updates ensure that the system is always in a consistent, functional state, with seamless rollback options for added reliability.
- **Reproducible Builds for Trust and Transparency:** With **Ignite**, rlxos guarantees fully reproducible builds, ensuring that every user gets the same, verifiable system environment.

### Why not rlxos?

- **Limited Customization for Power Users:** The immutable root filesystem restricts direct modifications, which might not appeal to users seeking complete control over system configuration.
- **Developing Ecosystem:** While rlxos is stable and reliable, it may lack some of the ecosystem maturity found in more established Linux distributions.

### Ignite: Buildtool for rlxos

**Ignite** is the powerful build tool used by rlxos to ensure **full reproducibility** across all system components. Whether updating or building from source, Ignite guarantees that **identical binaries** are produced every time, offering unparalleled trust and consistency.

#### Benefits:
- **Guaranteed Reproducibility:** Every build of rlxos produces the same binaries, ensuring a consistent and stable environment for all users.
- **Streamlined Debugging and Issue Resolution:** With a reproducible system, bugs and issues can be pinpointed and resolved more efficiently, thanks to the consistent environment.
- **Enhanced Security and Trustworthiness:** Reproducible builds provide a transparent system that reduces the risk of unauthorized changes or tampering.
