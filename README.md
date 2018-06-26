# OpenEdge ABL Snippets for VS Code

This extension for Visual Studio Code adds snippets for OpenEdge ABL.

## Installation

In order to install an extension you need to launch the Command Pallete (Ctrl + Shift + P or Cmd + Shift + P) and type Extensions.
There you have either the option to show the already installed snippets or install new ones. Search for *OpenEdge ABL Snippets* and install it.

## Snippets

Below is a list of all available snippets and the triggers of each one. The **⇥** means the `TAB` key.

### Define variable
| Trigger  | Content |
| -------: | ------- |
| `dvch⇥` | `DEFINE VARIABLE varName AS CHARACTER NO-UNDO.`|
| `dvin⇥` | `DEFINE VARIABLE varName AS INT64 NO-UNDO.` |
| `dvhn⇥` | `DEFINE VARIABLE varName AS HANDLE NO-UNDO.` |
| `dvda⇥` | `DEFINE VARIABLE varName AS DATE NO-UNDO.` |
| `dvde⇥` | `DEFINE VARIABLE varName AS DECIMAL NO-UNDO.` |
| `dvdt⇥` | `DEFINE VARIABLE varName AS DATETIME NO-UNDO.` |
| `dvlg⇥` | `DEFINE VARIABLE varName AS LOGICAL NO-UNDO.` |
| `dvlc⇥` | `DEFINE VARIABLE varName AS LONGCHAR NO-UNDO.` |
| `dvmp⇥` | `DEFINE VARIABLE varName AS MEMPTR NO-UNDO.` |

### Define input parameter
| Trigger  | Content |
| -------: | ------- |
| `ipch⇥` |`DEFINE INPUT  PARAMETER varName AS CHARACTER NO-UNDO.`|
| `ipin⇥` |`DEFINE INPUT  PARAMETER varName AS INT64 NO-UNDO.` |
| `iphn⇥` |`DEFINE INPUT  PARAMETER varName AS HANDLE NO-UNDO.` |
| `ipda⇥` |`DEFINE INPUT  PARAMETER varName AS DATE NO-UNDO.` |
| `ipde⇥` |`DEFINE INPUT  PARAMETER varName AS DECIMAL NO-UNDO.` |
| `ipdt⇥` |`DEFINE INPUT  PARAMETER varName AS DATETIME NO-UNDO.` |
| `iplg⇥` |`DEFINE INPUT  PARAMETER varName AS LOGICAL NO-UNDO.` |
| `iplc⇥` |`DEFINE INPUT  PARAMETER varName AS LONGCHAR NO-UNDO.` |
| `ipmp⇥` |`DEFINE INPUT  PARAMETER varName AS MEMPTR NO-UNDO.` |

### Define output parameter
| Trigger  | Content |
| -------: | ------- |
| `opch⇥` |`DEFINE OUTPUT PARAMETER varName AS CHARACTER NO-UNDO.`|
| `opin⇥` |`DEFINE OUTPUT PARAMETER varName AS INT64 NO-UNDO.` |
| `ophn⇥` |`DEFINE OUTPUT PARAMETER varName AS HANDLE NO-UNDO.` |
| `opda⇥` |`DEFINE OUTPUT PARAMETER varName AS DATE NO-UNDO.` |
| `opde⇥` |`DEFINE OUTPUT PARAMETER varName AS DECIMAL NO-UNDO.` |
| `opdt⇥` |`DEFINE OUTPUT PARAMETER varName AS DATETIME NO-UNDO.` |
| `oplg⇥` |`DEFINE OUTPUT PARAMETER varName AS LOGICAL NO-UNDO.` |
| `oplc⇥` |`DEFINE OUTPUT PARAMETER varName AS LONGCHAR NO-UNDO.` |
| `opmp⇥` |`DEFINE OUTPUT PARAMETER varName AS MEMPTR NO-UNDO.` |

### Define input-output parameter
| Trigger  | Content |
| -------: | ------- |
| `iopch⇥` |`DEFINE INPUT-OUTPUT PARAMETER varName AS CHARACTER NO-UNDO.`|
| `iopin⇥` |`DEFINE INPUT-OUTPUT PARAMETER varName AS INT64 NO-UNDO.` |
| `iophn⇥` |`DEFINE INPUT-OUTPUT PARAMETER varName AS HANDLE NO-UNDO.` |
| `iopda⇥` |`DEFINE INPUT-OUTPUT PARAMETER varName AS DATE NO-UNDO.` |
| `iopde⇥` |`DEFINE INPUT-OUTPUT PARAMETER varName AS DECIMAL NO-UNDO.` |
| `iopdt⇥` |`DEFINE INPUT-OUTPUT PARAMETER varName AS DATETIME NO-UNDO.` |
| `ioplg⇥` |`DEFINE INPUT-OUTPUT PARAMETER varName AS LOGICAL NO-UNDO.` |
| `ioplc⇥` |`DEFINE INPUT-OUTPUT PARAMETER varName AS LONGCHAR NO-UNDO.` |
| `iopmp⇥` |`DEFINE INPUT-OUTPUT PARAMETER varName AS MEMPTR NO-UNDO.` |

### All different
| Trigger  | Content |
| -------: | ------- |
| `ds⇥` |  `DEFINE STREAM streamName.`|
| `dvb⇥` | `DEFINE BUFFER bufferName FOR tableName.` |
| `ffwn⇥` | `FIND FIRST {table} WHERE {where} NO-LOCK NO-ERROR.` | 
| `i++⇥` | `$1 = $1 + 1.` |
| `i--⇥` | `$1 = $1 - 1.` |
| `&gl⇥` | `&GLOBAL-DEFINE $1` |
| `&sc⇥` | `&GLOBAL-DEFINE $1` |
| `123qw` | `23423432` |

### dtt⇥ - DEFINE TEMP-TABLE

```
DEFINE TEMP-TABLE ttName NO-UNDO
   FIELD fieldName AS dataType
.
```

### pro⇥ - DEFINE PROCEDURE

```
/*-----------------------------------------------------------------------------
  Purpose:     
  Parameters:  
  Notes:       
-----------------------------------------------------------------------------*/
PROCEDURE procName PRIVATE:
   ...
END PROCEDURE.
```

### func⇥ - DEFINE FUNCTION
```
/*-----------------------------------------------------------------------------
  Purpose:     
  Parameters:  
  Notes:       
-----------------------------------------------------------------------------*/
FUNCTION functionName RETURNS dataType PRIVATE (  ):
   DEFINE VARIABLE vRet   AS dataType NO-UNDO.
   ...
   RETURN vRet.
END FUNCTION.
```

### if⇥ - IF THEN
```
IF logicalExpression THEN DO:
   ...
END.
```

### ife - IF THEN ELSE
```
IF logicalExpression THEN DO:
   ...
END.
ELSE DO:
   ...
END.
```

