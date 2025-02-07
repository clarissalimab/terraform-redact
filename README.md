# terraform-redact
Run Terraform commands and anonymize account IDs on outputs and on `.tf` files.

## Installation

Run:

```bash
bin/install
```

## Usage

1. Replace raw account IDs with `$AWS_ACCOUNT_ID` on `.tf` files and export your AWS account ID:

```bash
export AWS_ACCOUNT_ID=123456789012
```

> [!TIP]
> You can also set the `AWS_ACCOUNT_ID` on your `.bashrc` or `.zshrc` file to avoid having that information on your shell history.

2. Run Terraform commands:
```bash
rtf init
rtf plan
rtf apply
```
