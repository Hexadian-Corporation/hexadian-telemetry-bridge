# hexadian-telemetry-bridge

A minimal native bridge, written in Rust, that relays the local telemetry
stream of Star Citizen to the Hexadian web applications running in a browser
on the same machine.

This repository is public so that anyone can read the code that runs on their
computer.

## What it does

- Connects to the telemetry service the game exposes on the local machine.
- Relays to the Hexadian web application, on the same machine, only the
  telemetry fields that the application asked for.
- Starts when the web application asks for it and stops when told to, or when
  no application is connected.

## What it does not do

- It does not process, store or upload anything.
- It does not send anything outside the local machine.
- It does not send commands to the game: it only reads.
- It does not read game files or logs.

## Status

Design stage. There is no released version yet.

## Contributions

This repository is read-only for the public. Issues and outside pull requests
are not accepted. Only the code owners listed in `CODEOWNERS` can change it.

## Security

See `SECURITY.md`.

## License

PolyForm Noncommercial License 1.0.0 (Modified). See `LICENSE`.

This project is not affiliated with or endorsed by Cloud Imperium Games.
Star Citizen is a trademark of its owner.
