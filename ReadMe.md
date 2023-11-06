# Linux-Container-Application-Using-Windows-Authenticated-NuGet-Package-Example

This is an example of one way to handle a container build pipeline, from a Linux build-agent, for an application with a NuGet-package dependency to a Windows-authenticated NuGet-server. Exemplified with ProGet, https://proget.example.org.

This is just an example made public. The code will not build because there is an invalid NuGet-reference and an invalid NuGet-server url. The pipelines will not run on GitHub. The repository needs to be located in an Azure DevOps on-premise. "example.org" is used instead of a real domain.

The package gss-ntlmssp/gssntlmssp needs to be installed on the Linux build-agent:

	apt update && apt install -y gss-ntlmssp

or

	sudo dnf update && sudo dnf install gssntlmssp

or maybe something else.

I am a bit of a Linux newbie.

- [Use private windows-authenticated NuGet-server from Azure DevOps Linux build-agents](https://hanskindberg.wordpress.com/2023/11/01/use-private-windows-authenticated-nuget-server-from-azure-devops-linux-build-agents/)