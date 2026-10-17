# Research notes

## Research question

How does ransomware affect data integrity and system access, and what host activity can help explain or detect those changes?

## Approach

The report brings together a literature review, ransomware case studies, and discussion of host behavior. It describes simulated encrypted files, benign encrypted files, and isolated virtual-machine scenarios. No live malware needs to be run to build the planned file-analysis tool.

The main behaviors discussed are rapid file modification, extension changes, increased file entropy, backup removal, and unusual disk activity.

## Case studies

**WannaCry:** The report discusses its spread, file encryption, and disruption to services.

**NotPetya:** The report uses it as an example of destructive behavior that can make recovery impossible, rather than a reliable pay-and-decrypt process.

## Findings

The research connects encryption with the wider effect on a host. Files may become inaccessible, backup options may be lost, and normal work may stop. Recovery also needs checks that restored data and the system can be trusted.

## Limits

The report contains example code and comparison figures, but the source scripts, datasets, and test logs have not been supplied for this repository. Its numerical comparisons are not presented here as independently reproduced measurements.

Entropy alone cannot separate ransomware from normal encryption or compression. A future implementation needs several indicators and tests for false positives.

## Next steps

1. Build a read-only file-analysis tool.
2. Prepare harmless test files, including compressed and encrypted examples.
3. Record entropy and file-change behavior.
4. Compare results and document false positives.
5. Add the code, tests, and instructions to this repository.
