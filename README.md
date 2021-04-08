**FMC ACP - Delete disabled rules and generate report script**

A python based script to generate report if there are disabled rules FMC ACP and delete disabled rules in bulk

The usage is as below.

Ensure python3 is installed and the below modules are already available. 

Both the python files "python delete_disabled_rule.py" and "rule_writer.py" is needed.

1. Enter the IP of the FMC
2. Username and password (Make use of a separate user for running API based script on FMC)
3. Select the ACP you want to delete disabled rules.
4. You can either choose to just generate the report or 
5. Generate report along with deleting the disabled rules and save the changes. 

```
    PS C:\Users\anpavith\OneDrive\Desktop\scripts\Delete_Disabled_Rules\Development\main_1.1> python delete_disabled_rule.py
    ###########################################################
    #               ACCESS CONTROL POLICY                     #
    ###########################################################
    #         anpavith              Cisco Systems India       #
    ###########################################################
    ###########################################################
    #             ACCESS CONTROL POLICY LIST                  #
    ###########################################################
    1 5585-SFR
    2 before_optima_copy
    3 Blank Policy
    4 Copy of Delhi Shared
    5 FTD-Mig-ACP-1613142830
    6 FTD-Mig-ACP-1615773808
    7 HELIUM
    8 Helium_COPY
    9 SERVER-FW-ZoneFree
    10 SERVER-FW-ZoneFree-Before-Optima
    11 BERLIN MASTERFIREWALL-Updated
    ###########################################################
    Choose the ACP Number (integer value):10
    ###########################################################
                    Available operations on ACP
    ###########################################################
    1. Report of rules which are disabled
    2. Delete disabled rules
    ###########################################################
    Enter your selection (integer value) : 2
    ###########################################################
    Processing, Please Wait
    >>>>>>>>
    Retrived all rules from  OLY-PCI-SERVER-FW-ZoneFree-Before-Optima
    ###########################################################
    Total number of rules in Access Control Policy  :  7965
    Number of rules which are disabled              :  154

    ###########################################################
    auth token--> d5f01051-08d3-4776-8d84-ab9f2e38bfc0
    refresh token--> 6f9991ce-b739-4f71-ac9d-10d7e5f5b040
    Successfully refreshed authorization token
    ###########################################################
    Processing, Please Wait!
    Delete was successful!
    Delete was successful!
    Delete was successful!
    Delete was successful!
    Delete was successful!
    Delete was successful!
    Delete was successful!
    Delete was successful!
    ###########################################################
```
