<!--
    {
        "name":"Generate an RSA key pair",
        "description":"Generate an RSA key pair and get the key's values and fingerprint"
    }
-->

_**IMPORTANT:** If you already have an RSA key pair in PEM format (minimum 2048 bits) and a fingerprint of the public key, you can skip this optional task and proceed to **Task 6**. To get your user's and tenancy's OCID, see [Where to Get the Tenancy's OCID and User's OCID](https://docs.oracle.com/en-us/iaas/Content/API/Concepts/apisigningkey.htm#five); however, going through the entire task might be easier for you as you can get all the information that you need from the **Configuration File Preview** dialog box when you create your keys._

## Introduction

In this task, you learn how to use the **Console** to generate the private/public key pair. If you already have a key pair, you can choose to upload the public key instead. The **Console** also displays the _configuration file preview_ dialog box that contains important information such as the **user ocid**, **tenancy ocid**, **region**, and the generated **fingerprint** private and/or public key values.

+ An RSA key pair in PEM format (minimum 2048 bits). See [How to Generate an API Signing Key](https://docs.oracle.com/en-us/iaas/Content/API/Concepts/apisigningkey.htm#two).
+ The fingerprint of the public key. See [How to Get the Key's Fingerprint](https://docs.oracle.com/en-us/iaas/Content/API/Concepts/apisigningkey.htm#four).
+ The user's and tenancy's OCIDs. See [Where to Get the Tenancy's OCID and User's OCID](https://docs.oracle.com/en-us/iaas/Content/API/Concepts/apisigningkey.htm#five).

Estimated Time: 5 minutes

1. In the **Console** banner, click the **Profile** icon. From the drop-down menu, click your **My profile**.

    ![Click the person icon at the far upper right and click your username.](./images/click-my-profile.png " ")

2. The **My profile** page is displayed. In the **User Information** tab, you can click the **Copy** link next to the **OCID** field. Make a note of this username's OCID as you will need it in a later task. Scroll down the page to the **Resources** section, and then click **API Keys**.

    ![Click Auth Tokens under Resources at the bottom left.](./images/click-api-key.png " ")

3. In the **API Keys** section, click **Add API Key**. The **Add API Key** dialog box is displayed.

    ![Click Add API Key.](./images/click-add-api-key.png " ")

4. Click **Download private key**. The private key is downloaded to your Web browser's default directory such as the **Downloads** folder in MS-Windows. A checkmark is displayed next to the **Download private key**.

    ![Download private key.](./images/download-private-key.png " ")

    The name of the downloaded private key is usually as follows:

    **`oraclecloudidentityservice_username-date.pem`**

    Rename your downloaded private key to something shorter such as:

    **`oci-api-private-key.pem`**

5. You can download the public key if you need it or for potential future use. click **Download Public Key**. The public key is downloaded to your Web browser's default directory such as the **Downloads** folder in MS-Windows. A checkmark is displayed next to the **Download Public Key**.

6. A checkmark should appear next to each button. Click **Add**. The key is added and the **Configuration File Preview** dialog box is displayed. The file snippet includes required parameters and values you'll need to create your configuration file.

    ![Configuration file preview.](./images/config-file-preview.png " ")

    This dialog box contains all of the information that you will need in the next task to create a new Cloud location and credential. Click the **Copy** link to copy the **User's OCID**, **API Key Fingerprint**, and **Tenancy OCID** to your clipboard and then paste it into a text editor of your choice such as Notepad in MS-Windows. You will need those values in the next task.

    ![Credentials items.](./images/credentials-items.png " ")

    You can access the downloaded private key and then paste the key value in the above text editor file as you will need the value in the next task.

    ![Private key value.](./images/get-private-key-value.png " ")

7. In the **Configuration File Preview** dialog box, click **Close**.

## Want to Learn More?

* [Oracle Cloud Infrastructure Documentation](https://docs.cloud.oracle.com/en-us/iaas/Content/GSG/Concepts/baremetalintro.htm)
* [Overview of Oracle Cloud Infrastructure Identity and Access Management](https://docs.cloud.oracle.com/en-us/iaas/Content/Identity/Concepts/overview.htm)

## Acknowledgements

* **Author:** Lauran Serhal, Consulting User Assistance Developer
* **Last Updated By/Date:** Lauran Serhal, February 2024