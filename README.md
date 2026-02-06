# Delphi and Free Pascal/Lazarus Comparison
A developer-oriented comparison of Delphi and Free Pascal/Lazarus, covering platforms, tooling, workflows, and project fit.


## Section A - Quick Decision Matrix

### Project & Platform Scenarios

| Scenario                               | Delphi                   | FPC / Lazarus                  | Notes                                                                                                                                                                                                                                        |
| -------------------------------------- | ------------------------ | ------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Commercial Windows desktop application | **Strongly recommended** | **Viable**                     | Delphi excels in IDE productivity, VCL ecosystem, and long-term ISV support                                                                                                                                                                  |
| Cross-platform desktop application     | **Recommended**          | **Recommended**                | Delphi (FMX) emphasizes productivity; FPC/Lazarus emphasizes openness and flexibility                                                                                                                                                        |
| Mobile apps (iOS / Android)            | **Strongly recommended** | **Supported (advanced setup)** | Delphi provides an integrated mobile framework (FMX); FPC supports native mobile targets via cross-compilation but relies on custom or community tooling                                                                                     |
| Linux server / middle-tier services    | **Recommended**          | **Strongly recommended**       | Both are well-suited; Delphi shines in shared-code business backends, FPC in lightweight services and infrastructure tools                                                                                                                   |
| Command-line tools (CLI)               | **Recommended**          | **Strongly recommended**       | FPC commonly used for small, fast, low-dependency binaries                                                                                                                                                                                   |
| Embedded system host / HMI software    | **Strongly recommended** | **Recommended**                | Targets embedded or industrial systems running a full OS (Windows or Linux). Delphi excels at rapid UI development and device integration; FPC/Lazarus is well-suited for cross-platform or open deployments                                 |
| Embedded / bare-metal targets          | **Not supported**        | **Strongly recommended**       | Targets systems without a general-purpose OS (microcontrollers, SoCs with no OS or minimal RTOS). Requires custom startup code, memory layout control, and direct hardware access. FPC supports minimal runtimes and bare-metal environments |
| Open-source  projects                  | **Recommended**          | **Strongly recommended**       | FPC has no licensing cost and broad platform freedom                                                                                                                                                                                         |
| Commercial ISV products                | **Strongly recommended** | **Viable**                     | Delphi’s tooling, support, and ecosystem favor commercial development                                                                                                                                                                        |

### Legend

- **Strongly recommended** – Excellent fit; commonly chosen with low friction
- **Recommended** – Solid fit; used successfully in production
- **Supported (advanced setup)** – Technically supported but requires significant manual setup
- **Viable** – Possible, but notable trade-offs exist
- **Not supported** – No practical or supported solution

---
### Notes

- **Delphi** prioritizes productivity, tooling integration, and commercial application development on full operating systems.
- **FPC / Lazarus** prioritizes platform breadth, openness, and low-level control, often at the cost of higher setup effort.
- In many scenarios, *both* toolchains are viable; the deciding factors are usually **time-to-solution**, **licensing**, and **deployment constraints**.

*This matrix is intended as a starting point. Detailed feature comparisons follow in later sections.*

---


