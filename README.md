Automated Trader for The Chartist
=================================


**Automated Trader for The Chartist** software is for trading [**US Power Setups**](https://www.thechartist.com.au/Benefits/short-term-share-trading.html) provided by [**The Chartist**](https://www.thechartist.com.au/). The software is provided **FREE OF COST**.

**The software comes with**:

* Host of simplified features for trading with [Interactive Brokers](http://www.interactiverbrokers.com) via IB Gateway API connectivity
* One click process for downloading, processing, placing and reporting of **The Chartist**'s [US Power Setups](https://www.thechartist.com.au/Benefits/short-term-share-trading.html) (activation license key required)
* Set and forget hands-free feature for performing the one-click process automatically everyday at a designated time [*disabled feature*]
* Active monitoring of placed orders [*coming soon*]

*Warning: In this version of the software, the orders are not actively monitored. If you are using MARGIN greater than 1.0 please be aware that US HFT orders are not actively monitored. The next version of this software will be shipped with active monitoring feature.*

**Requirements**:

* Windows operating systems ( XP or higher)
* .NET Environment (usually Win7 onwards the operating systems comes pre-loaded with .NET environment)
* Internet Explorer (version 9 or higher)
* stable Internet connection (minimum speed 500kbps)
* Account with [Interactive Brokers](http://www.interactivebrokers.com) for trading
* [Interactive Brokers Trader Workstation or Gateway](https://www.interactivebrokers.com/en/index.php?f=14099#tws-software)
* Subscription to **The Chartist**'s [US Power Setups](https://www.thechartist.com.au/Benefits/short-term-share-trading.html) (_required only if you wish to use **The Chartist** auto-trade feature_)

**Download**:
Visit [Automated Trader for The Chartist](http://www.theportfoliotrader.com/downloads/automated-trader-for-the-chartist/) to download this software.

> **Note**:
> * Please use a valid email address while registering to download the software.
> * License key will be generated and emailed to your email address. You will have to input this license key when prompted during the first run.
> * The software is made available with single-computer license i.e. locked to one computer.
> * In case you want to run this software on multiple computers then increase the number of license's required during the registration process or contact info@theportfoliotrader.com for assistance.
> * Dependency on Internet Explorer is temporary, I have included it so that the user can visualise the website login and file access actions.
> * _This application should run fine on LINUX and OS X/Mac OS via [Mono](http://www.mono-project.com/). Due to the dependency of this version on Internet Explorer it might be a difficult ask. I have not tested this thoroughly. Contact info@theportfoliotrader.com if you want me to perform a thorough testing on LINUX or OS X/Mac OS. Next version of this software will not have Internet Explorer dependency._
> * **DISCLAIMER**: Automated Trader for The Chartist is dependent upon the design and/or organisation of the [The Chartist](https://www.thechartist.com.au)'s website, delivery and format of trades as of today. In an event, where [The Chartist](https://www.thechartist.com.au)'s website and/or delivery and format of trades has been re-designed or re-organised, then auto-trade functionality may or may not work untill modifications have been made to this software to accomodate such changes. 

<br>
<br>


<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

Table of Contents
-----------------
[Automated Trader for The Chartist](#automated-trader-for-the-chartist)
  - [Architecture](#architecture)
  - [Features](#features)
    - [Interactive Brokers (IB) connectivity](#interactive-brokers-ib-connectivity)
    - [The Chartist](#the-chartist)
  - [How To](#how-to)
    - [Set Up](#set-up)
      - [Install](#install)
      - [First Run](#first-run)
    - [Connect to IB gateway](#connect-to-ib-gateway)
    - [Subscribe to account information](#subscribe-to-account-information)
    - [Close open positions](#close-open-positions)
    - [Place or modify orders](#place-or-modify-orders)
      - [Changing extended ticker attributes](#changing-extended-ticker-attributes)
      - [Changing extended order attributes](#changing-extended-order-attributes)
    - [Cancel orders](#cancel-orders)
    - [Check executions](#check-executions)
    - [The Chartist: Set Trade Settings](#the-chartist-set-trade-settings)
    - [The Chartist: Set TPT Web Settings](#the-chartist-set-tpt-web-settings)
    - [The Chartist: Set Report Settings](#the-chartist-set-report-settings)
    - [The Chartist: One-Click Process](#the-chartist-one-click-process)
    - [The Chartist: Orders & Log Diary](#the-chartist-orders--log-diary)
    - [The Chartist: Report Format](#the-chartist-report-format)
  - [Support](#support)
  - [License](#license)
  - [Risk Disclosure Statement](#risk-disclosure-statement)

> _Note_: _Table of Contents_  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


<br>
<br>


##Architecture
-----------------
The architecture of this software is presented in the figure below:

<br>
![Automated Trader for The Chartist](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/AutomatedTrader_Diagram.png)

:arrow_double_up: [Back to Top](#table-of-contents)

<br>
<br>

##Features
----------


### Interactive Brokers (IB) connectivity
This provides a simplified user-interface and connectivity to Interactive Brokers gateway. All settings are stored locally on your computer. Every time the application is loaded, these settings are retrieved for your convenience.
 
* **Connection**
    * Connection status indicator
    * Connect to IB Gateway by setting IP address, log level, port number and client id including Connect and Disconnect buttons
    * Log: Server logs, Error logs, Clear error log button

 ![Connection](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/tab_connection.png)

<br>
    
* **Account** 
    * Account number indicator
    * Last sync time indicator
    * Subscribe, Unsubscribe and Clear Account Summary buttons
    * Summary and Portfolio tabs
    * Close Position by right-click on Portfolio

    ![Account](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/tab_account.png)

<br>

* **Order**
    * Ticker description and Order description (including extra Ticker attributes and Order attributes)
    * What-If, Place Orders, GLOBAL CANCEL, Clear Orders buttons
    * Next Order-ID in-sync with IB Gateway
    * Open Orders and Order Status tab
    * Cancel Order by right-click on Open Orders

    ![Orders](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/tab_orders.png)

<br>

* **Executions**
    * Executions request settings
    * Request Executions and Clear Executions button
    * Reports tab

    ![Executions](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/tab_executions.png)

<br>
    
* **Settings**
   * All settings i.e. connection, ticker and order settings saved in an XML file (ibSet.xml)
   * Every time the application loads, it will retrieve settings from the settings XML file

<br>

* **In-Sync**
   *  Always in-sync with IB Gateway i.e. whenever IB Gateway delivers data, all logs, account summary, portfolio changes, order status changes are updated


:arrow_double_up: [Back to Top](#table-of-contents)


<br>
<br>

###The Chartist
This provides a user-interface to alter settings for trading using [**The Chartist**](https://www.thechartist.com.au)'s [**US Power Setups**](https://www.thechartist.com.au/Benefits/short-term-share-trading.html) and to perform one-click trading. All settings are stored locally on your computer, using strong encryption where required. Every time the application is loaded, these settings are retrieved for your convenience.

* **Trade Settings**
   * Set paths for downloaded files
   * Manage your trade details such as exchange, position size, margin, etc.

<br>
   
* **The Chartist Login**
    * Your login details for **The Chartist**'s [US Power Setups](https://www.thechartist.com.au/Benefits/short-term-share-trading.html)

<br>

* **Report Settings**
    * Set your **To** and **From** email and its mail settings for report delivery

<br>
    
* **Process**
    * One-Click processing for downloading, order management, placing orders and report generation

<br>

* **Orders, Log Diary and Log**
	* List of day's orders and log diary of orders
	* Process log to keep you up-to-date on the current process pipeline
 
  ![Auto Trade](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/tab_tc.png)

<br>
* **Safety Checks**
	* [The Chartist](https://www.thechartist.com.au)'s trades are never processed more than once
	* Account capital is always retrieved based on the currency settings
	* Check for duplicate orders
	* BUY order will not be placed if an OPEN position already exists in your portfolio
	* SELL order will not placed if an OPEN position does not exist in your portfolio (No Short Selling)
	* Orders are double-checked, before being placed, to match your position-size
	* All BUY orders are placed **@ LMT** and all SELL orders are placed **@ MKT**
	* Your portfolio OPEN positions are matched with [The Chartist](https://www.thechartist.com.au)'s OPEN positions:
		* if your portfolio has an OPEN position that [The Chartist](https://www.thechartist.com.au) does not have, then a SELL order is generated to close that position
		* if your portfolio **does not** have an OPEN position that [The Chartist](https://www.thechartist.com.au) has, then **BUY ORDER IS NOT GENERATED**
  
  
:arrow_double_up: [Back to Top](#table-of-contents)

<br>
<br>

## How To

### Set Up

#### Install
* You will download a **.zip** from the [download area](#download)
* Extract the **.zip** file to your chosen location, a new folder titled **TPT Automated Trader** will be created. For example, I have extracted the **.zip** to **D:\** drive

![first_open](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/firstrun_open.png)

<br>

#### First Run
* Double click on **TradingAutomation.exe**
* Enter license key when prompted

![license_key](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/firstrun_key_2.png)

>**Note**:
> * License keys are emailed to your email address when you downloaded the software.
> * It is not mandatory to input the license key. However, **The Chartist** auto-trade facility will be only be activated for valid licenses. In case of invalid license key, you will have access to all other facility i.e. Interactive Brokers Gateway interface, but not **The Chartist** auto-trade facility. You will have the option of activating **The Chartist** auto-trade option using **Activate The Chartist** button on the **Connection** tab.

:arrow_double_up: [Back to Top](#table-of-contents)


<br>
<br>

### Connect to IB gateway
* Log in to your IB account via IB Gateway or Trader Workstation
* Go to **Connection** tab
* Click **Connect** (usually the default setting provided will work, unless IB TWS/Gateway API settings are different to default setting)

![connect](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/2_connect.png)

>**Note**:
> * [Instructions on to how to enable connectivity on your IB Gateway or Trader Workstation](https://github.com/virusme/Automated-Trader-for-NSE/wiki/IB-API-Settings) 
> * IB Trader Workstation is a full-featured trading platform, it requires lots of memory and needs restart every 24 hours. Whereas IB Gateway is headless (no user-interface) connectivity to IB servers, it requires minimal memory and does not need restarts that often.
> * To use with Automated Trader for The Chartist, I recommend IB Gateway because it is light-weight and does not need restarts
>* Server and error logs provide a log of IB server requests and any error reports that IB Server reports or that arise due to connection with IB Server
> ![servererr](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/2_servererrlogs.png)


:arrow_double_up: [Back to Top](#table-of-contents) 

<br>
<br>

### Subscribe to account information
* Go to **Account** tab
* Click **Subscribe**

![account](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/2_subscribe.png)


:arrow_double_up: [Back to Top](#table-of-contents)

<br>
<br>


### Close open positions
* Go to **Account** :arrow_right: **Portfolio** tab
* Right-click on the open position that you intend to close
* Click **Close Position**

![closepos](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/2_portfolio_closepos.png)


:arrow_double_up: [Back to Top](#table-of-contents)

<br>
<br>


### Place or modify orders
* Go to **Orders** tab
* Click **Place/Modify Order**
* A pop dialog opens up where you can enter your order details and click **Place/Modify Order**

![placeorder](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/2_place_orders.png)


:arrow_double_up: [Back to Top](#table-of-contents)

<br>
<br>


#### Changing extended ticker attributes
* Go to **Orders** :arrow_right: **Place/Modify Order**
* Click **Ext. Ticker Attr.**
* Make changes if required and click **Apply**

![placeorder_extticker](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/2_place_orders_extticker.png)

<br>

#### Changing extended order attributes
* Go to **Orders** :arrow_right: **Place/Modify Order**
* Click **Ext. Order Attr.**
* Make changes if required and click **Apply**

![placeorder_extorder](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/2_place_orders_extorders.png)


>**Note**:
>* For definition and description of each of the parameters in ticker attributes or order attributes please visit [Interactive Brokers knowledge base](https://ibkb.interactivebrokers.com/)
>* Default settings work fine for day orders
>* Every time **Apply** is clicked, the settings are saved automatically for future use. These settings are retrieved whenever the application is loaded, for your convenience.
>* **GLOBAL CANCEL** cancels all open orders in one go.


:arrow_double_up: [Back to Top](#table-of-contents)

<br>
<br>


### Cancel orders
* Go to **Orders** :arrow_right: **Open Orders** tab
* Right click on the order that you wish to cancel and select **Cancel Order**

![placeorder_cancel](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/_placed_order_cancel.png)


:arrow_double_up: [Back to Top](#table-of-contents)

<br>
<br>


### Check executions
* Go to **Executions** tab
* Click **Request Executions**
* In case, you want to retreive the execution report of a particular order, use the form provided to fill in the details before clicking **Request Executions**

![reqexe](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/2_reqexecutions.png)

>**Note**:
>* Interactive Brokers provide execution report for the day (24 hours) and the **Report** table is always in-sync with IB data. Therefore, in most cases you will rarely have to **Request Executions** as they are delivered to this software as and when IB reports it.


:arrow_double_up: [Back to Top](#table-of-contents)

<br>
<br>


### The Chartist: The Chartist Login Details
The login and password provided here will be used to login to https://www.thechartist.com.au website.

* Go to **The Chartist** :arrow_right: **Settings**  tab
* Click **The Chartist Login Details**
* You should enter your login and password that you use to access **The Chartist**'s [US Power Setups](https://www.thechartist.com.au/Benefits/short-term-share-trading.html)
* This data is stored locally on your computer using strong encryption for future use

![tc_web](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/_tc_tclog.png)


:arrow_double_up: [Back to Top](#table-of-contents)

<br>
<br>


### The Chartist: Trade Settings
The data provided in this setting will be used by auto-trader for determining your choice of [US Power Setups](https://www.thechartist.com.au/Benefits/short-term-share-trading.html), security type, exchange, position size, etc.
These settings need to be set once. The settings are saved locally for future use. 

#### The Chartist: Select US Power Setup Strategy

* Go to **The Chartist** :arrow_right: **Settings** tab
* Select a strategy from the drop-down menu as shown in the figure below

<br>

![tc_select](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/_tc_select.png)

<br>

#### The Chartist: Set Trade Settings

* Go to **The Chartist** :arrow_right: **Settings** tab
* Click **Settings**
* Make changes as required and click **Apply**
*  Default settings work well
*  Definition of terms:
  * **File Path**: Location or a directory where you want the downloaded files to be saved. If left empty, the default is the folder the application is running in.
  * **Markey**:  NASDAQ( default). The exchange this auto-trade will be working on
  * **Currency**: USD (default). The currency this auto-trade will be utilising
  * **Sec. Type**: STK (default). The security type this auto-trade will be trading
  * **Leverage**: 1.0 (default). The leverage/margin you wish to use.
  * **Allocation**: 100% (default). The percentage of capital you wish to auto-trade with. For example, if you have USD 100K, and set **Allocation** as 60%, then only USD 60K will be used for auto-trade
  * **Position Size**: 6.5% (default). The percentage of allocated capital per position
  * **Max. Amount**: 2000000 (default). Any high number you wish, this is used to make sure no *crazy* orders are placed on the market

![tc_trade](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/_tc_tcset.png)

>**Note**:
>* Do not change settings under **The Chartist Sheet**, automated trader will not work if you change this setting
>* Standard ticker and order attributes for trading [US Power Setups]() (both Original and HFT) is stored locally on your computer. They can be viewed by opening either _utilities/sys.xml_ or _utilities/hft.xml_ using a word-processor
>* Every time **Apply** is clicked, the settings are saved for future use


:arrow_double_up: [Back to Top](#table-of-contents)

<br>
<br>



### The Chartist: Set Report Settings
The data provided here will be used for generating and saving reports, as well as emailing the report to your chosen email address.

* Go to **The Chartist** :arrow_right: **Settings** tab
* Click **Report Settings**
* Make changes as required and click **Apply**
* Definition of terms:
  * **From-Email Settings**
     * **Email Address**:  An email address that you own from which you want to send email from
     * **Password**: Password to the above email-address
     * **Custom Email Subject**: A tag or an identifier that will be prefixed to the subject of the email for your identification at the other end. You can chose to leave this empty.
  * **Mail Settings**: This setting will let your computer know how to send the email
     * **SMTP**: SMTP address of your from-email address provider. The one shown in the figure below is from **GMAIL**
     * **Port**: Port number settings for your from-email address provider. The one shown in the figure below is from **GMAIL**
   * **To-Email Settings**
      * **To Email Address**: An email address that you may/may not own to which you want the email with report attached to be sent to

![tc_report](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/_tc_repset.png)

>**Note**:
>* To send an email, one needs an email address where the email originates (from-email) and a destination email (to-email)
>* **From-Email** and **To-Email** could be the same email address
>* Every time **Apply** is clicked, the settings are saved for future use

:arrow_double_up: [Back to Top](#table-of-contents)


<br>
<br>


### The Chartist:  One-Click Process
This will download your chosen [**US Power Setup**](https://www.thechartist.com.au/Benefits/short-term-share-trading.html), check account information, process orders, manage orders, generate new orders to be placed, place orders to IB server, prepare a detailed report of this processing and email the report.
During the execution of this process, Internet Explorer will open automatically to help you visualise the logging in to The Chartist and accessing [**US Power Setups**](https://www.thechartist.com.au/Benefits/short-term-share-trading.html) actions. Internet Explorer will close by itself once the process is completed.

<p align="center">
WARNING: DO NOT FORCIBLY CLOSE INTERNET EXPLORER WHILE THE PROCESS IS RUNNING.
</p>
 
* Go to**The Chartist** :arrow_right: **Settings** tab
* Click **Process**
* And that's it!

Figure below presents the auto-trade in action:

<br>
![tc_inaction](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/_tc_inaction.png)


<br>
![tc_process](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/_tc_process.png)

>**Note**:
>* The figure above shows the detailed process log


:arrow_double_up: [Back to Top](#table-of-contents)

<br>
<br>


###The Chartist: Orders & Log Diary
Details of order management, daily orders and daily log (number of orders, file downloaded, etc.) will displayed here at the end of  [One-Click Process](#the-chartist-one-click-process)

To View details of order management and daily orders:
* Go to **The Chartist** :arrow_right: **Orders**

![tc_orders](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/_tc_orders.png)

To View details of daily logs:
* Go to **The Chartist** :arrow_right: **Log Diary**

![tc_logdiary](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/_tc_logdiary.png)


:arrow_double_up: [Back to Top](#table-of-contents)

<br>
<br>


###The Chartist: Report Format

![tc_report](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/_tc_report.png)

The report that will generated and emailed would consist of:

* *Summary*: Summary of your account and placed orders
* *Process Log*: Process log of auto-trade
* *Log Diary*: Daily log of number of buy, sell, open positions and comments
* *The Chartist Orders*: The Chartist orders for the day
* *Portfolio*: A snapshot of your portfolio at the time of processing
* *API Error Logs*: Error log from the IB server

![tc_reportemail](https://github.com/virusme/Automated-Trader-for-The-Chartist/blob/master/screenshots/_tc_reportemail.png)

Above is an example of the report-email format:

* *Email Subject*: The email has a subject that is composed of three parts. The first part is the name of the application that is sending this report, the second part is **Custom Email Subject** from your [Report Settings](#the-chartist-set-report-settings) and the third part is the status message of the process.
* *Attachment*: The report file is attached to the email
* *Email Body*: The email body consists of a generic message. However, if there were errors during the processing, those errors are listed in the body for your convenience. 

>**Note**:
>* The reports are also saved on your local computer in the directory where this application resides under **reports** directory
>* Reports are organised in **MMYYYY** folder with **ddMMYYY.xlsx** format, for example report for **19th February 2016** will be under **reports/022016/** and the file name would be **19022016.xlsx**


:arrow_double_up: [Back to Top](#table-of-contents)

<br>
<br>


Support
---------
Contact info@theportfoliotrader.com for assistance or if you have any queries.


<br>
<br>


License
----------
<p align="justify">
All the computer programs and software are supplied with the explicit understanding that they are to be used only for purposes that the computer programs and software were built for, as stated by the provider. It is expressly prohibited to misuse the software by any individual, organisation, firm, limited liability company or private limited company.

Full terms and conditions of downloading this software will be displayed when you are about to download the software.

</p>
By downloading or using the programs, you acknowledge acceptance of the following DISCLAIMER OF WARRANTY:

<p align="center">
DISCLAIMER OF WARRANTY
</p>
<p align="justify">
ALL THE COMPUTER PROGRAMS AND SOFTWARE ARE PROVIDED "AS IS" WITHOUT WARRANTY OF ANY KIND. WE MAKE NO WARRANTIES, EXPRESS OR IMPLIED, THAT THEY ARE FREE OF ERROR, OR ARE CONSISTENT WITH ANY PARTICULAR STANDARD OF MERCHANTABILITY, OR THAT THEY WILL MEET YOUR REQUIREMENTS FOR ANY PARTICULAR APPLICATION. THEY SHOULD NOT BE RELIED ON FOR SOLVING A PROBLEM WHOSE INCORRECT SOLUTION COULD RESULT IN INJURY TO A PERSON OR LOSS OF PROPERTY. IF YOU DO USE THEM IN SUCH A MANNER, IT IS AT YOUR OWN RISK. THE USE OF THIS SOFTWARE FOR ACTUAL TRADING IS AT YOUR OWN RISK. THE AUTHOR AND PUBLISHER DISCLAIM ALL LIABILITY FOR DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES RESULTING FROM YOUR USE OF THE PROGRAMS.
</p>

<br>

###Interactive Brokers API
C# API is provided by [Interactive Brokers](http://www.interactivebrokers.com). Please refer to [Interactive Brokers](http://www.interactivebrokers.com) for any licensing terms and conditions of their API.

**DISCLAIMER**: Automated Trader for The Chartist software is not endorsed by [Interactive Brokers](http://www.interactivebrokers.com) or any of its affiliates. 

<br>

###The Chartist
Subscription to **The Chartist**'s [US Power Setups](https://www.thechartist.com.au/Benefits/short-term-share-trading.html) is provided by [The Chartist](https://www.thechartist.com.au/). Please refer to [The Chartist](https://www.thechartist.com.au/) for terms and conditions.

**DISCLAIMER**: Automated Trader for The Chartist software is not endorsed by [The Chartist](https://www.thechartist.com.au) or any of its affiliates.

**DISCLAIMER**: Automated Trader for The Chartist is dependent upon the design and/or organisation of the [The Chartist](https://www.thechartist.com.au)'s website, delivery and format of trades as of today. In an event, where [The Chartist](https://www.thechartist.com.au)'s website and/or delivery and format of trades has been re-designed or re-organised, then auto-trade functionality may or may not work untill modifications have been made to this software to accomodate such changes. 
 
<br>

Risk Disclosure Statement
-------------------------------
<p align="justify">
THE RISK OF LOSS IN TRADING SECURITIES AND LEVERAGED INSTRUMENTS CAN BE SUBSTANTIAL. YOU SHOULD THEREFORE CAREFULLY CONSIDER YOUR OBJECTIVES, FINANCIAL SITUATION, NEEDS AND ANY OTHER PERSONAL CIRCUMSTANCES TO DETERMINE WHETHER SUCH TRADING IS SUITABLE FOR YOU.

HIGH LEVERAGE OF LEVERAGE IS OFTEN OBTAINABLE. YOU SHOULD BE AWARE THAT THE USE OF LEVERAGE CAN LEAD TO LARGE LOSSES AS WELL AS GAINS.

THIS BRIEF STATEMENT CANNOT DISCLOSE ALL OF THE RISKS AND OTHER SIGNIFICANT ASPECTS OF SECURITIES AND DERIVATIVES MARKETS. THEREFORE, YOU SHOULD CONSULT YOUR FINANCIAL ADVISOR OR ACCOUNTANT TO DETERMINE WHETHER TRADING IN SECURITES AND DERIVATIVES PRODUCTS IS APPROPRIATE FOR YOU IN LIGHT OF YOUR FINANCIAL CIRCUMSTANCES.
</p>
<br>
:arrow_double_up: [Back to Top](#table-of-contents)