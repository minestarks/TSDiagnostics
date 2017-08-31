To collect diagnostics on Windows:

1. Save https://raw.githubusercontent.com/minestarks/TSDiagnostics/master/wpr/tsevents.wprp to your local drive.
2. Open an administrator command prompt and navigate into the folder where you just saved `tsevents.wprp`.
3. Run the following to start tracing:
```wpr -start tsevents.wprp```
4. Reproduce the problem (by opening TypeScript files, typing, etc.)
5. Run the following to stop tracing:
```wpr -stop tstraces.etl```
6. Share the resulting `tstraces.etl` with the person who requested more information.

_WARNING:_ The trace file `tstraces.etl` may contain identifying information. Be wary of sharing publicly.