Download the CIS-CAT tool 

https://www.cisecurity.org/cybersecurity-tools/cis-cat-pro/cis-benchmarks-supported-by-cis-cat-pro/
https://it.stonybrook.edu/help/kb/downloading-and-using-cis-cat-benchmarks-tool


Unzip the tool and run in the Linux 



usage: Assessor-CLI.[bat|sh] -[options] <extras>
---------------------------------------------------------------------------------------------------
 Options                                           Tip
---------------------------------------------------------------------------------------------------
 -b,--benchmark <BMK-OR-DSC>                       Path to file containing assessment content, such
                                                   as an XCCDF or DataStream Collection
 -bi,--benchmark-info                              When used with -b, display information about the
                                                   selected benchmark or datastream collection, such
                                                   as a profile listing
 -cfg,--config-xml <CONFIGURATION XML FILE>        Path to an XML configuration file detailing
                                                   assessments to perform against various sessions.
 -cl,--checklist <CHECKLIST>                       Used only when the -b argument selects a
                                                   <data-stream-collection> document for assessment,
                                                   the -cl option selects the ID of the specific
                                                   checklist to assess
 -csv                                              Generate report results in CSV format
 -D <property=value>                               Customize user properties or interactive values
 -dm,--data-stream <DATA-STREAM>                   Used only when the -b argument selects a
                                                   <data-stream-collection> document for assessment,
                                                   the -dm option selects the ID of the specific
                                                   data-stream to assess
 -e,--encrypt <FILE TO ENCRYPT>                    Full path to the a sessions.properties file or
                                                   configuration.xml file to be encrypted, including
                                                   the file name and its extension
 -ep,--encryption-password <ENCRYPTION PASSWORD>   The password that will be used to encrypt a
                                                   sessions.properties file or configuration.xml
                                                   file
 -fp,--file-password <FILE PASSWORD>               The password originally used to encrypt a
                                                   sessions.properties file or configuration.xml
                                                   file
 -gui                                              The assessment is run by the GUI
 -h,--help                                         Show usage information
 -html                                             Generate report results in HTML format
 -i,--interactive                                  Proceed interactively
 -json                                             Generate report results in JSON format
 -l,--list                                         List available assessment content
 -lv,--list-verbose                                Add verbose output when listing available content
 -narf,--no-arf                                    Do not generate report results in Asset Reporting
                                                   Format
 -nl,--no-logging                                  Disable all logging (Default log level is WARN)
 -npr                                              Generate a JSON report showing results that did
                                                   not pass (fail, error, unknown)
 -nrf,--no-report-file                             Do not generate an assessment report file.  This
                                                   option is intended to be used in conjunction with
                                                   the -u option.  If the -u option is not
                                                   specified, the assessment results will be saved
                                                   as a file regardless.
 -nts,--no-timestamp                               Do not include the auto-generated timestamp as
                                                   part of the report name.
 -o,--definitions                                  Definitions/Vulnerability Assessment
 -od,--oval-definitions <OVAL DEFINITIONS>         Path to file containing OVAL Definitions
 -ov,--oval-variables <OVAL VARIABLES>             Path to file containing OVAL Variables
 -p,--profile <PROFILE>                            ID/Name of the specific profile to assess
 -props,--properties <PROPERTIES-FILE>             Location (absolute or relative to starting
                                                   directory) of custom Assessor properties file
 -q,--quiet                                        Quiet Mode: Disable assessment status output
 -rd,--reports-dir <REPORTS-DIR>                   Path to a directory specifying the location to
                                                   which output reports are saved
 -rp,--report-prefix <REPORT-PREFIX>               Override the default report name.  Timestamp
                                                   information will be appended to the report
                                                   prefix, except when the -nts option is included
                                                   as well.
 -sessions,--sessions <SESSIONS.PROPERTIES>        Location (absolute or relative to starting
                                                   directory) of Sessions configuration file
 -test,--test                                      Used in conjunction with the 'sessions' option,
                                                   or with the default 'sessions.properties' file,
                                                   test the validity of session configurations,
                                                   reporting success or failure
 -txt                                              Generate report results in plain-text format
 -u,--url <REPORTS-URL>                            Sends a HTTP POST with the Assessment Results XML
                                                   to the specified URL
 -ui,--ignore-warnings                             Ignore certificate warnings when POSTing results
                                                   to a URL.
 -v,--error                                        Configure log level to ERROR
 -vdd,--vulnerability-definitions                  Download the latest vulnerability definitions
 -vv,--warn                                        Configure log level to WARN
 -vvv,--info                                       Configure log level to INFO
 -vvvv,--debug                                     Configure log level to DEBUG
 -vvvvv,--trace                                    Configure log level to TRACE
 -vvvvvv,--all                                     Configure log level to ALL
---------------------------------------------------------------------------------------------------

Examples:
Run the tool in an interactive mode and export the report to /var/www/html/index.html                                                    
sh ./Assessor-CLI.sh -i -rd /var/www/html/ -nts -rp index                                                    
                                                     
                                                     
                                                     
                                                     
