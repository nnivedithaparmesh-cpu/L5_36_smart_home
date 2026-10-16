\# Static Code Analysis – Issue Table



| Issue | Type | Line(s) | Description | Fix Approach |

|---|---|---|---|---|

| Unsafe subprocess execution with `shell=True` | Bandit – High | Original code | Shell execution can allow command injection. | Removed the unsafe subprocess usage. |

| Binding to all network interfaces (`0.0.0.0`) | Bandit – Medium | Original code | Exposes the service on all available network interfaces. | Changed the host to `127.0.0.1` for local access. |

| Mutable default argument `{}` | Pylint | Original code | A mutable default can be shared across function calls. | Used `None` and initialized a new dictionary inside the function. |

| Missing function docstrings | Pylint | Multiple | Functions lacked descriptions. | Added docstrings. |

| Inconsistent naming and formatting | Pylint / Flake8 | Multiple | Naming and whitespace did not follow conventions. | Used consistent naming and corrected formatting. |

| File opened without an explicit encoding | Pylint | Original code | File encoding was not specified. | Used `encoding="utf-8"`. |

| Hardcoded password | Bandit – Low | Original code | A password was embedded in the source. | Removed the hardcoded password. |



\## Verification Results



\- Pylint: improved from 4.80/10 to 10.00/10.

\- Bandit: no issues reported after fixes.

\- Flake8: no violations reported after fixes.

