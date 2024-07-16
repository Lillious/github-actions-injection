## GitHub Actions Command Injection

###### <i>This repository is used to demonstrate a command injection vulnerability within GitHub Actions. This is known by GitHub but they have refused to fix it.</i>

### Usage:
- Fork the repository
- Open the Actions tab of the forked repository
- Select the workflow <b>GitHub Actions Injection Action</b>
- Click the <b>Run Workflow &#9660;</b> dropdown
- Input the below example command

```ps
";systeminfo"
```

###### Observe GitHub's lack of input sanitation when passing in variables, as quotes are removed from user input automatically.