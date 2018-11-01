paramiko

API Documentation

Core SSH protocol classes

1) client
import paramiko

calling client.py

1)paramiko.client.AutoAddPolicy



Flow
paramiko const ==> from paramiko.client 

from paramiko.client import (
    SSHClient,
    MissingHostKeyPolicy,
    AutoAddPolicy,
    RejectPolicy,
    WarningPolicy,
)

all classes present in the client


client = paramiko.client.SSHClinet()  /// SSHClinet class ==> construbctor call
///  sshclinet class calling the function present init

SSHClient
  - load_system_host_keys()
  - load_host_keys
  - get_host_keys
  - set_log_channel
  - set_missing_host_key_policy
  - connect()
  - exec_command()
  - invoke_shell
  - open_sftp
  - get_transport
  - _auth()







