# Integration for ICD 10/11 to DHIS2

## Requirements

* Java 11+

## Building & Starting

```bash
sh ./start.sh
```

## Commands

### icd11

```bash
NAME
	icd11 - Generate DHIS2 OptionsSet with ICD11 codes and saves the output to a file

SYNOPSYS
	icd11 [[--root-id] string]  [[--release-id] string]  [[--linearization-name] string]  [[--language] string]  [[--host] string]  [[--client-id] string]  [[--client-secret] string]  [[--file-out] string]  [--verbose]  

OPTIONS
	--root-id  string
		ICD Entity ID to start with
		[Optional, default = ]

	--release-id  string
		ICD 11 Release Id. One of 2021-05, 2020-09, 2019-04, 2018
		[Optional, default = 2021-05]

	--linearization-name  string
		Short name for the linearization. e.g. mms for ICD Mortality and Morbidity Statistics
		[Optional, default = mms]

	--language  string
		Language for entity descriptions. One of ar, en, es, zh
		[Optional, default = en]

	--host  string
		Host of the ICD11 repository. The default value works with docker approach
		[Optional, default = http://localhost]

	--client-id  string
		
		[Optional, default = The client id to be used with the publicly hosted icd1 repository]

	--client-secret  string
		
		[Optional, default = The client secret to be used with the publicly hosted icd1 repository]

	--file-out  string
		Path to the output file
		[Optional, default = options.json]

	--verbose	Indicates whether progress should be displayed verbosely
		[Optional, default = false]

```