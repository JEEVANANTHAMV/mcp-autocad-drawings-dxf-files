# AutoCAD Drawings (DXF Files)

> Reads, writes, and checks AutoCAD drawing (DXF) files directly. You don't need AutoCAD installed to use it — only to open the results afterwards.

The bundle zip (**55.9 MB**) is stored in this repository at **`6e3c0250-88a6-428f-8d14-7836b26cb82a.zip`**.

This repository is part of the **Forjinn-Desk** MCP bundle collection. An MCP bundle is a self-contained server that a host application launches and communicates with over the MCP (Model Context Protocol) protocol.

## Repo metadata

| Field | Value |
| --- | --- |
| Registry ID | `6e3c0250-88a6-428f-8d14-7836b26cb82a` |
| Status in registry | active |
| Bundle size | 55.9 MB |
| Distribution | committed to this repo |

## Environment variables

| Variable | Value / note |
| --- | --- |
| `DXF_WORKDIR` | `__INSTALL_DIR__` |

## MCP launch configuration

The host replaces `__INSTALL_DIR__` (install dir) and `__PYTHON__` (bundled Python) at runtime.

```json
{
  "command": "__PYTHON__",
  "args": [
    "server.py"
  ],
  "env": {
    "DXF_WORKDIR": "__INSTALL_DIR__"
  }
}
```


## Install / usage

1. Get the bundle:
   - download `6e3c0250-88a6-428f-8d14-7836b26cb82a.zip` from this repo (Code → Download ZIP, or `git clone`).
2. Extract to your target installation directory (config paths expect contents at the install-dir root).
3. Set the environment variables listed above.
4. Launch using the MCP config JSON (or let a host client manage it automatically).

> Bundles may include vendored runtimes (bundled Python, Node, or native executables). Builds are Windows x64.
