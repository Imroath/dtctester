FROM mcr.microsoft.com/dotnet/framework/sdk:4.8-windowsservercore-ltsc2016

WORKDIR /dtctester

COPY /files .

ENV MSDTC_SQLSERVER_HOSTNAME sqlserver
ENV MSDTC_SQLSERVER_PORT 1433
ENV MSDTC_SQLSERVER_USER sa
ENV MSDTC_SQLSERVER_PASSWORD Passw0rd
ENV MSDTC_TEST_DATABASE ODBCTest
ENV ACCEPT_EULA=Y

CMD ["powershell", ".\\entrypoint.ps1", "-Verbose"]