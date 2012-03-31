# Ignore-Patterns for VCS
The plan is to collect ignore patterns for different Version Control Systems here.

## Git
The simplest thing is to run wget:

    wget https://raw.github.com/lcorneliussen/xignore/master/.gitignore --no-check-certificate
    
Or, as an alternative download it with powershell:

    [System.Net.ServicePointManager]::ServerCertificateValidationCallback = {$true}; 
    (new-object System.Net.WebClient).DownloadFile( "https://raw.github.com/lcorneliussen/xignore/master/.gitignore", ".\.gitignore" )