
### Using the Pelastic tool

#### Download
https://github.com/codingogre/pelastic/archive/master.zip

#### Configuration
Pelastic requires a configuration file, where the path (including file) is either pulled from the environment variable `PELASTIC_CONFIG`,
or looked for in the hard-coded `~/.config/pelastic.ini`

Example on Apple OS X.  Open the Terminal.app and enter the following
```bash
export PELASTIC_CONFIG=$HOME/pelastic.ini
```

Example on Windows.  Open Powershell and enter the following
```bash
[Environment]::SetEnvironmentVariable("PELASTIC_CONFIG", "C:\Users\wutan\pelastic.ini", "User")
```

Example Configuration File
```bash
[peloton]
username = Your_Peloton_Username_Or_Email
password = Your_Peloton_Password

[elastic]
id = Your_Elastic_Cloud_ID
username = Your_Elastic_Cluster_Username
password = Your_Elastic_Cluster_Password
```

#### Example Usage
Open the Terminal.app on Apple OS X and navigate to the folder where pelastic is downloaded

```bash
./pelastic.py
```

Open Powershell on Windows
```bash
python pelastic.py
```