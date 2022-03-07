#### NOTES:

##### February 2022 Data structure change

The content of submissions [changed](https://www.protondb.com/news/a-contribution-flow-for-2022) on February 18th, 2022 and this is reflected in data exports starting with the March 2022 export. The changes:

- Responses now formally specify `variant` of type: `'experimental' | 'ge' | 'native' | 'notListed' | 'official' | 'older'`.
- `protonVersion` is only now present in the case of `variant` being `older`
- `type` is no longer provided because it is now calculated dynamically by ProtonDB based on the responses. This would previously be one of `'steamPlay' | 'tinker'`.
- The `flow` response was pruned from export. This was for processing purposes and not from submitter input. In these exports it was always `proton`
- There are now additional responses:
 
```concludingNotes?: string
  customProtonVersion?: string
  launchOptions?: string
  triedOob?: Binary
  tinkerOverride?: Binary
  verdictOob?: Binary
```

##### October 2019 Questionnaire Change
The contribute workflow changed to a questionnaire on October 28, 2019, and this changed the structure of data exports beginning with the December 2, 2019 export. For the full set of reports, combine with the last export before this.
