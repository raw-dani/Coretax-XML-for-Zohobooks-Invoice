# Coretax XML Generator for Zoho Books Invoice

A Deluge script to generate Coretax-compatible XML files from Zoho Books invoices.

## Features

- Generates XML files compatible with Coretax format
- Handles multiple invoice line items
- Includes proper tax calculations
- Supports customer NPWP data
- Automatic email notifications with XML attachments

## Setup

1. Add the script to your Zoho Books custom function
2. Configure the following custom fields in Zoho Books Contacts:
   - cf_no_npwp
   - cf_nama_npwp 
   - cf_alamat_npwp

## Usage

The script will:
1. Process selected invoices
2. Generate XML with proper Coretax format
3. Send email with XML attachment
4. Return success code and XML data

## XML Format

The generated XML follows this structure:
- TaxInvoiceBulk
  - TIN
  - ListOfTaxInvoice
    - TaxInvoice
      - TaxInvoiceDate
      - BuyerInfo
      - ListOfGoodService
        - GoodService items

## Contributing

Feel free to submit issues and pull requests.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
