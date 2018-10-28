Simple report to show non-compliant junos versions.
For sake of time a number of values are hard coded.

Find and Report non compliant hosts
compReport.yml - finds non compliant junos versions and saves to junosVer.yml to be used as variables later.

Generate Report
generateReport.yml - takes junosVerTemplate.j2 and junosVer.yml and creates a html file junosReport.html to display non compliant hosts and junos version being used.

To view results 
Open Report Display.PNG or
Open junosReport.html in browser


Hosts and Versions used in lab

ok: [172.16.1.41] => {
    "msg": "SRX1  15.1X49-D140.2"
}

ok: [172.16.1.42] => {
    "msg": "SRX2  15.1X49-D140.2"
}

ok: [172.16.1.43] => {
    "msg": "SRX3  18.1R2.5"
}
