# Visit Management

A comprehensive Odoo module for managing customer visits and sales activities.

## About

An Odoo module that enables sales teams to track and manage customer visits with GPS location tracking capabilities.
It streamlines the sales process by allowing visits to be seamlessly converted into sales orders and quotations.

## Features

- **Customer Visit Tracking**: Create and manage customer visits with detailed notes and scheduling
- **GPS Location Tracking**: Automatically capture GPS coordinates, IP address, city, and country information when visits are submitted
- **Visit Status Management**: Track visit lifecycle through Draft, Submitted, Converted, and Cancelled states
- **Sales Order Integration**: Seamlessly convert visits into sales orders with a simple wizard
- **Multi-Company Support**: Full support for multi-company environments
- **Activity Tracking**: Built-in mail threading and activity management for collaboration
- **Role-Based Access Control**: Comprehensive security with user and manager roles
- **Automatic Numbering**: Sequential visit numbers for easy tracking and reference

## Installation

1. Place the module in your Odoo addons directory
2. Update the apps list in Odoo
3. Search for "Visit Management" in the Apps menu
4. Click Install

## Configuration

After installation, configure the module:

1. Go to **Sales → Configuration → Settings**
2. Scroll to the **Visit Management** section
3. Configure your preferences

## Usage

### Creating a Visit

1. Navigate to **Sales → Visits → Visits**
2. Click **Create**
3. Fill in the visit details:
   - Customer
   - Visit Date
   - Salesperson (auto-populated with current user)
   - Visit Notes
4. Click **Save**

### Submitting a Visit

1. Open a visit record
2. Click **Submit** to change the status to Submitted
3. GPS location data will be automatically captured if available

### Converting to Sales Order

1. Open a submitted visit
2. Click **Create Sales Order**
3. The wizard will pre-fill customer and salesperson information
4. Confirm to create the sales order
5. The visit status will change to "Converted to Sale"

## Technical Details

- **Module Name**: visit
- **Version**: 1.0
- **Category**: Sales
- **License**: LGPL-3
- **Dependencies**: base, sale, mail, web

### Models

- `visit.visit`: Main visit management model with GPS tracking
- `visit.make.sale`: Wizard for converting visits to sales orders
- Extended `sale.order`: Added relationship to track visits
- Extended `res.config.settings`: Configuration options for the module

## Support

For issues, questions, or contributions, please contact the module maintainer.

## Credits

**Author**: Your Name

**License**: LGPL-3