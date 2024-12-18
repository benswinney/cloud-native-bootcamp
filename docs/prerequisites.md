# Prerequisites

## Required skills

This activities contained here require you to be proficient in working from the command line with a linux shell (Bash, Zsh, etc.) Below is a partial list of activities you should be able to perform. 

- Copy, move, and rename files
- Understand linux file permissions
- Edit text files (vi, vim, emacs, etc)
- Edit environment variables ($PATH)

Here is a course for learning (or brushing up) on working from the linux command line [Linux Command Line Basics](https://www.udacity.com/course/linux-command-line-basics--ud595)

## Workstation Setup
=== "Openshift (MacOS/Linux)"

    ## Create accounts

    You'll need these accounts to use the Developer Tools environment.

    - [GitHub account](http://github.com) (public, not enterprise): Create one if you do not have one aleady. If you have not logged in for a while, make sure your login is working.

    - [IBM Cloud Account](https://cloud.ibm.com): Create one if needed, make sure you can log in. 

    - [O'Reilly Account](https://learning.oreilly.com/home/): The account is free and easy to create.

    - [RedHat Account](https://www.redhat.com/en): Needed for CodeReady Containers.

    ## Run System Check Script

    Run the following command in your terminal to check which tools need to be installed.

    Using `wget`:

    ```
    wget -O - https://cloudbootcamp.dev/scripts/system-check.sh | sh
    ```

    Using `curl`:

    ```
    curl -s https://cloudbootcamp.dev/scripts/system-check.sh | sh
    ```

    After the script is run, make sure to install any missing tools.

    ## Install CLIs and tools

    The following is a list of desktop tools required to help with installation and development.

    - [Git Client](https://git-scm.com/): Needs to be installed in your development operating system, it comes as standard for Mac OS

    - [IBM Cloud CLI](https://cloud.ibm.com/docs/cli?topic=cloud-cli-getting-started): Required for management of IBM Cloud Account and management of your managed IBM Kubernetes and Red Hat OpenShift clusters
        - Don't install just the [IBM Cloud CLI](https://cloud.ibm.com/docs/cli?topic=cloud-cli-install-ibmcloud-cli), install the [IBM Cloud CLI and Developer Tools](https://cloud.ibm.com/docs/cli?topic=cloud-cli-getting-started#step1-install-idt)
        ```
        curl -sL https://ibm.biz/idt-installer | bash
        ```

    !!! Note
        If you log in to the web UI using SSO, you'll need to [create an API key](https://cloud.ibm.com/docs/iam?topic=iam-federated_id) for logging into the CLI. 

    - [Podman Desktop](https://podman-desktop.io/): Required for building and running container images.
        - Installed and running on your local machine

    - [Tekton CLI](https://github.com/tektoncd/cli): Used to help control Tekton
    pipelines from the command line.
        ```
            brew tap tektoncd/tools
            brew install tektoncd/tools/tektoncd-cli
        ```

    - [Visual Studio Code](https://code.visualstudio.com/download): A popular code editor
        - You will be required to edit some files, having a good quality editor is always best practice
        - Enabling [launching VSCode from a terminal](https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line)

    - [JDK 11](https://www.oracle.com/technetwork/java/javase/downloads/jdk11-downloads-5066655.html): _Optional_ installed on your local machine
        - Used for SpringBoot content


=== "Openshift (Windows)"

    ## Create accounts

    You'll need these accounts to use the Developer Tools environment.

    - [GitHub account](http://github.com) (public, not enterprise): Create one if you do not have one aleady. If you have not logged in for a while, make sure your login is working.

    - [IBM Cloud Account](https://cloud.ibm.com): Create one if needed, make sure you can log in. 

    - [O'Reilly Account](https://learning.oreilly.com/home/): The account is free and easy to create.

    - [RedHat Account](https://www.redhat.com/en): Needed for CodeReady Containers.

    ## Cloud Native VM

    Use the [Cloud Native VM](https://github.com/csantanapr/vagrant-cloud-native#install) it comes pre-installed with kubernetes and all cloud native CLIs.

    Is highly recommended for Windows users to use this VM.

    ## Install CLIs and tools

    The following is a list of desktop tools required to help with installation and development.

    - [Git Client](https://git-scm.com/): Needs to be installed in your development operating system, it comes as standard for Mac OS

    - [IBM Cloud CLI](https://cloud.ibm.com/docs/cli?topic=cloud-cli-getting-started): Required for management of IBM Cloud Account and management of your managed IBM Kubernetes and Red Hat OpenShift clusters
        - Don't install just the [IBM Cloud CLI](https://cloud.ibm.com/docs/cli?topic=cloud-cli-install-ibmcloud-cli), install the [IBM Cloud CLI and Developer Tools](https://cloud.ibm.com/docs/cli?topic=cloud-cli-getting-started#step1-install-idt)
        ```
        curl -sL https://ibm.biz/idt-installer | bash
        ```

    !!! Note 
        If you log in to the web UI using SSO, you'll need to [create an API key](https://cloud.ibm.com/docs/iam?topic=iam-federated_id) for logging into the CLI. 

    - [Podman Desktop](https://podman-desktop.io/): Required for building and running container images.
        - Installed and running on your local machine

    - [Tekton CLI](https://github.com/tektoncd/cli): Used to help control Tekton pipelines from the command line.


    - [Visual Studio Code](https://code.visualstudio.com/download): A popular code editor
        - You will be required to edit some files, having a good quality editor is always best practice
        - Enabling [launching VSCode from a terminal](https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line)

    - [JDK 11](https://www.oracle.com/technetwork/java/javase/downloads/jdk11-downloads-5066655.html): _Optional_ installed on your local machine
        - Used for SpringBoot content

    - [OpenShift CodeReady Containers (CRC)](https://code-ready.github.io/crc/#installing-codeready-containers_gsg)

    <InlineNotification kind="warning">

    **Warning:** Make sure you have Cisco VPN turned off when using CRC.

    </InlineNotification>

=== "Kubernetes (MacOS/Linux)"
    ## Create accounts

    You'll need these accounts to use the Developer Tools environment.

    - [GitHub account](http://github.com) (public, not enterprise): Create one if you do not have one aleady. If you have not logged in for a while, make sure your login is working.

    - [IBM Cloud Account](https://cloud.ibm.com): Create one if needed, make sure you can log in. 

    - [O'Reilly Account](https://learning.oreilly.com/home/): The account is free and easy to create.


    ## Run System Check Script

    Run the following command in your terminal to check which tools need to be installed.

    Using wget:
    ```
    wget -O - https://cloudbootcamp.dev/scripts/system-check.sh | sh
    ```

    Using curl:
    ```
    curl -s https://cloudbootcamp.dev/scripts/system-check.sh | sh
    ```

    After the script is run, make sure to install any missing tools.

    ## Install CLIs and tools

    The following is a list of desktop tools required to help with installation and development.

    - [Git Client](https://git-scm.com/): Needs to be installed in your development operating system, it comes as standard for Mac OS

    - [IBM Cloud CLI](https://cloud.ibm.com/docs/cli?topic=cloud-cli-getting-started): Required for management of IBM Cloud Account and management of your managed IBM Kubernetes and Red Hat OpenShift clusters
        - Don't install just the [IBM Cloud CLI](https://cloud.ibm.com/docs/cli?topic=cloud-cli-install-ibmcloud-cli), install the [IBM Cloud CLI and Developer Tools](https://cloud.ibm.com/docs/cli?topic=cloud-cli-getting-started#step1-install-idt)
        ```
        curl -sL https://ibm.biz/idt-installer | bash
        ```

     !!! Note
        If you log in to the web UI using SSO, you'll need to [create an API key](https://cloud.ibm.com/docs/iam?topic=iam-federated_id) for logging into the CLI. 
    

    - [Podman Desktop](https://podman-desktop.io/): Required for building and running container images.
        - Installed and running on your local machine

    - [Tekton CLI](https://github.com/tektoncd/cli): Used to help control Tekton
    pipelines from the command line.
        ```
            brew tap tektoncd/tools
            brew install tektoncd/tools/tektoncd-cli
        ```

    - [Visual Studio Code](https://code.visualstudio.com/download): A popular code editor
        - You will be required to edit some files, having a good quality editor is always best practice
        - Enabling [launching VSCode from a terminal](https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line)

    - [JDK 11](https://www.oracle.com/technetwork/java/javase/downloads/jdk11-downloads-5066655.html): _Optional_ installed on your local machine
        - Used for SpringBoot content

    - [Minikube](https://kubernetes.io/docs/tasks/tools/install-minikube/): Follow the instructions for your Operating System.

    <InlineNotification kind="warning">

    **Warning:** Make sure you have Cisco VPN turned off when using minikube.

    </InlineNotification>

=== "Kubernetes (Windows)"

    ## Create accounts

    You'll need these accounts to use the Developer Tools environment.

    - [GitHub account](http://github.com) (public, not enterprise): Create one if you do not have one aleady. If you have not logged in for a while, make sure your login is working.

    - [IBM Cloud Account](https://cloud.ibm.com): Create one if needed, make sure you can log in. 

    - [O'Reilly Account](https://learning.oreilly.com/home/): The account is free and easy to create.

    ## Cloud Native VM

    Use the [Cloud Native VM](https://github.com/csantanapr/vagrant-cloud-native#install) it comes pre-installed with kubernetes and all cloud native CLIs.

    Is highly recommended for Windows users to use this VM.

    ## Install CLIs and tools

    The following is a list of desktop tools required to help with installation and development.

    - [Git Client](https://git-scm.com/): Needs to be installed in your development operating system, it comes as standard for Mac OS

    - [IBM Cloud CLI](https://cloud.ibm.com/docs/cli?topic=cloud-cli-getting-started): Required for management of IBM Cloud Account and management of your managed IBM Kubernetes and Red Hat OpenShift clusters
        - Don't install just the [IBM Cloud CLI](https://cloud.ibm.com/docs/cli?topic=cloud-cli-install-ibmcloud-cli), install the [IBM Cloud CLI and Developer Tools](https://cloud.ibm.com/docs/cli?topic=cloud-cli-getting-started#step1-install-idt)
        ```
        curl -sL https://ibm.biz/idt-installer | bash
        ```

    !!! Note
        If you log in to the web UI using SSO, you'll need to [create an API key](https://cloud.ibm.com/docs/iam?topic=iam-federated_id) for logging into the CLI. 


    - [Podman Desktop](https://podman-desktop.io/): Required for building and running container images.
        - Installed and running on your local machine

    - [Tekton CLI](https://github.com/tektoncd/cli): Used to help control Tekton
    pipelines from the command line.
        ```
            brew tap tektoncd/tools
            brew install tektoncd/tools/tektoncd-cli
        ```

    - [Visual Studio Code](https://code.visualstudio.com/download): A popular code editor
        - You will be required to edit some files, having a good quality editor is always best practice
        - Enabling [launching VSCode from a terminal](https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line)

    - [JDK 11](https://www.oracle.com/technetwork/java/javase/downloads/jdk11-downloads-5066655.html): _Optional_ installed on your local machine
        - Used for SpringBoot content

    - [Minikube](https://kubernetes.io/docs/tasks/tools/install-minikube/): Follow the instructions for your Operating System.

    <InlineNotification kind="warning">

    **Warning:** Make sure you have Cisco VPN turned off when using minikube.

    </InlineNotification>


## Environment Setup 
=== "MiniKube"

    - Verify your cluster has 4GB+ memory, and kubernetes 1.16+
        ```
        minikube config view
        ```
    - Verify your `vm-driver` is set for `hyperkit`
        ```
        minikube config set vm-driver hyperkit
        ```
    - In case memory is not set, or need to increase set the memory and recreate the VM
        ```
        minikube config set memory 4096
        minikube config set kubernetes-version v1.16.6
        minikube delete
        minikube start
        ```
    - Kubernetes should be v1.15+
        ```
        kubectl version
        ```

=== "OpenShift Local"

    Make sure OpenShift Local is installed. Check out the [OpenShift Local](https://docs.redhat.com/en/documentation/red_hat_openshift_local/2.44/html/getting_started_guide/index){target="_blank"} Page.

    ** Setup CRC **
    ```
    crc setup
    ```
    ** Start CRC **
    ```
    crc start
    ```
=== "IKS"

    - Login to [IBM Cloud](https://cloud.ibm.com) with your IBM ID.

    - Click "Create Resource" and search for "kubernetes service".

    - Select the tile for "Kubernetes Service" and do the following:
    - Select the "Free Cluster" plan.
    - Name your cluster.
    - Select "Create" at the bottom right of the screen.

    - Once the Cluster is provisioned, Click on the "Connect via CLI" in the top right corner.

    - Follow the instructions to connect and you are set to go.

=== "OpenShift on IBM Cloud (4.x)"

    - In this approach you share an OpenShift cluster on IBM Cloud with other bootcamp attendees.

    - Considering 10-15 attendees we recommend a cluster with 3 worker nodes (each 8 vCPUs + 32GB RAM - b3c.8x32).

    - Ask your IBM cloud account owner to provide access to an OpenShift cluster.

    - In addition to the IBM Cloud CLI also install the [OpenShift Origin CLI](https://cloud.ibm.com/docs/openshift?topic=openshift-openshift-cli#cli_oc) to be able to execute all commands.

    - Open your OpenShift web console from within your IBM cloud account, select your profile and choose "copy login command" to retrieve an access token for the login.

    - Login with your OpenShift Origin CLI.
        ```
        oc login --token=<token> --server=<server-url>:<server-port>
        ```

    - Create your own project / namespace in OpenShift that you will leverage across all labs.
        ```
        oc new-project <dev-your_initials>
        ```

    - Validate in the OpenShift web console that your project has been created (Administrator view -> Home -> Projects)


## Next Steps
Once Setup is complete, you can now begin reading our about [Cloud Native](./cloud-native/index.md by clicking the link, or the `Next` button below.
