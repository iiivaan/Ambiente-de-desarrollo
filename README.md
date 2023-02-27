# Ambiente-de-desarrollo

Microsoft Windows [Versión 10.0.19045.2604]
(c) Microsoft Corporation. Todos los derechos reservados.

C:\WINDOWS\system32>git clone https://github.com/wjfatuan/envcheck
Cloning into 'envcheck'...
remote: Enumerating objects: 47, done.
remote: Counting objects: 100% (47/47), done.
remote: Compressing objects: 100% (34/34), done.
remote: Total 47 (delta 19), reused 33 (delta 11), pack-reused 0
Receiving objects: 100% (47/47), 10.08 KiB | 3.36 MiB/s, done.
Resolving deltas: 100% (19/19), done.

C:\WINDOWS\system32>cd envcheck

C:\Windows\System32\envcheck>envecheck.bat
"envecheck.bat" no se reconoce como un comando interno o externo,
programa o archivo por lotes ejecutable.

C:\Windows\System32\envcheck>envcheck.bat

C:\Windows\System32\envcheck>echo -- Running environment tests
-- Running environment tests

C:\Windows\System32\envcheck>pip install pipenv
"pip" no se reconoce como un comando interno o externo,
programa o archivo por lotes ejecutable.

C:\Windows\System32\envcheck>pipenv install pytest
"pipenv" no se reconoce como un comando interno o externo,
programa o archivo por lotes ejecutable.

C:\Windows\System32\envcheck>pipenv run pytest -rA envcheck.py  1>test_results.txt
"pipenv" no se reconoce como un comando interno o externo,
programa o archivo por lotes ejecutable.

C:\Windows\System32\envcheck>git add *

C:\Windows\System32\envcheck>git commit -m "Submitting results"
Author identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'sofia camelo@Sofii.(none)')

C:\Windows\System32\envcheck>git push

Excepción no controlada: System.ComponentModel.Win32Exception: El nombre del directorio no es válido
   en System.Diagnostics.Process.StartWithCreateProcess(ProcessStartInfo startInfo)
   en System.Diagnostics.Process.Start()
   en GitCredentialManager.GitProcess.get_Version()
   en GitCredentialManager.GitProcessConfiguration.GetCanonicalizeTypeArg(GitConfigurationType type)
   en GitCredentialManager.GitProcessConfiguration.TryGet(GitConfigurationLevel level, GitConfigurationType type, String name, String& value)
   en GitCredentialManager.GitConfigurationExtensions.TryGet(IGitConfiguration config, String name, Boolean isPath, String& value)
   en GitCredentialManager.Settings.<GetSettingValues>d__5.MoveNext()
   en System.Linq.Enumerable.FirstOrDefault[TSource](IEnumerable`1 source)
   en GitCredentialManager.Settings.TryGetSetting(String envarName, String section, String property, String& value)
   en GitCredentialManager.Authentication.MicrosoftAuthentication.CanUseBroker(ICommandContext context)
   en GitCredentialManager.Program.Main(String[] args)
Username for 'https://github.com':
