# Splunkbase Download Utility

This utility provides a convenient method for Splunk administrators to download Splunkbase apps via the command line using a Python3 script. 

## Installation

Simply download the script and make it executable:
```
wget https://raw.githubusercontent.com/marcusschiesser/splunkbase-download/main/download-splunkbase.py
chmod +x ./download-splunkbase.py
```

Call then `./download-splunkbase.py` to get help how to use the script.

If needed, install the requirements:
```
pip install $(curl -s https://raw.githubusercontent.com/marcusschiesser/splunkbase-download/main/requirements.txt)
```

## History 

It's inspired by [https://github.com/tfrederick74656/splunkbase-download](https://github.com/tfrederick74656/splunkbase-download)
which unfortunately wasn't working anymore with `sid` and `SSOID` authentication as [Splunk changed the authentication method](https://github.com/tfrederick74656/splunkbase-download/issues/1). 
I initially fixed that, but then Splunk again changed the authentication (Please stop doing that!).
Kudos to [torhment](https://github.com/Tohrment) - he helped out and fixed it again in his [download_splunkbase_app](https://github.com/Tohrment/download_splunkbase_app). I merged his approach to my app too as our both apps have a slightly different usage interface. Mine is used by the [splunk-gitops](https://github.com/marcusschiesser/splunk-gitops) project.

## Disclaimer

This utility uses a service provided by Splunk. Please read the following prior to use:

 - Splunk® is a trademark or registered trademark of Splunk Inc. in the United States and other countries.
 - Use of the Splunk website is subject to the [Splunk Website Terms and Conditions of Use](https://www.splunk.com/view/SP-CAAAAAH).
 - Apps from Splunkbase are individually licensed and subject to the terms and conditions of their respective licenses.
 - The author of this tool takes no responsibility for your use of Splunk products and services.
 
By using this utility, you acknowledge that you have read and understand all of the above statements and agree to abide and be bound by them.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.