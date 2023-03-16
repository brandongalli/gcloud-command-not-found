# gcloud-command-not-found
Explains how to fix `command not found: gcloud` error

Once you download and unzip `gcloud sdk`, you will need to install and initialize `gcloud sdk`.
- `./google-cloud-sdk/install.sh` 

  **Note: Please make sure you answered Yes(`Y`) to prompt `Modify profile to update your $PATH and enable bash completion? (Y/n)`.
  If not, I recommend you to reinstall `gcloud` SDK.**
- `./google-cloud-sdk/bin/gcloud init`


After that, you might get command not found error for `gcloud`.
Here is how you can fix the error.
- Once we look around the downloaded sdk directory we might notice that it conatins some `path.*.inc` and `completion.*.inc`.
- Depending on your terminal(bash or zsh), you can run the below commands:
  
  * Bash
    
    ```
    source [path-to-download]/google-cloud-sdk/path.bash.inc
    source [path-to-download]/google-cloud-sdk/completion.bash.inc
    ```
  * Zsh
  
    ```
    source [path-to-download]/google-cloud-sdk/path.zsh.inc
    source [path-to-download]/google-cloud-sdk/completion.zsh.inc
    ```
  
  
