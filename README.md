# python3-nmap GUI for Beginners

> [!IMPORTANT]
> **Archived / no longer actively maintained.**
>
> This repository is preserved as a historical beginner-oriented example of wrapping Nmap with Python and a desktop GUI. No further feature development or compatibility maintenance is planned.

## Historical purpose

The example in `python3nmap_gui.py` combines:

- `python3-nmap` / `nmap3`
- FreeSimpleGUI
- a locally installed Nmap executable

The original GUI screenshot is retained in `GUI_IMAGE.webp`.

## Final dependency snapshot

For reproducibility, the final archived Python dependency snapshot is recorded in `requirements.txt`:

- `python3-nmap==1.9.1`
- `FreeSimpleGUI==5.3.0.post1`

The historical PySimpleGUI import has been replaced with the open-source FreeSimpleGUI fork for the final archived snapshot. This repository does **not** claim that every historical widget/behavior has been revalidated against that release.

Install the recorded Python dependencies with:

```console
python -m pip install -r requirements.txt
```

You must also install **Nmap** separately on the operating system.

## Operational caveats

Some Nmap operations require elevated privileges. Historical functions in this repository include OS detection, SYN/FIN/UDP scans, subnet scanning, ping scanning, version detection, and related Nmap operations. Only scan systems and networks you are authorized to test.

This archive does not perform live-network CI because Nmap behavior depends on the host OS, installed Nmap version, permissions, and network environment.

## References

- python3-nmap: https://pypi.org/project/python3-nmap/
- FreeSimpleGUI: https://pypi.org/project/FreeSimpleGUI/
- Nmap: https://nmap.org/

## Repository status

No further dependency automation, CodeQL schedules, bot-driven maintenance, or feature work is planned. The repository is intended to remain public and read-only after GitHub archival.
