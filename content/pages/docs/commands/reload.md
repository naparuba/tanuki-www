Title: Commands: Reload
Slug: docs/commands/reload


# XXX Reload

Command: `XXX reload`

The leave command triggers a reload of configuration files for the agent.

The `SIGHUP` signal is usually used to trigger a reload of configurations,
but in some cases it may be more convenient to trigger the CLI instead.

This command operates the same as the signal, meaning that it will trigger
a reload, but does not wait for the reload to complete. Any errors with the
reload will be present in the agent logs and not in the output of this command.

## Usage

Usage: `XXX reload`

The command-line flags are all optional. The list of available flags are:

* `-rpc-addr` - Address to the RPC server of the agent you want to contact
  to send this command. If this isn't specified, the command will contact
  "127.0.0.1:8400" which is the default RPC address of a XXX agent.

