### Introduction & Definition

This section is already clear and sets the context. Let's move on to the specifics.

### Automated Translation Services

**Automated Translation Service (ATS) Implementation:**

1. **Setup and Integration:**
    - Integrate AWS Machine Translations (Amazon Translate) into your development workflow.
    - Ensure you have the appropriate AWS credentials and API keys securely stored and managed.
2. **String Identification:**
    - Ensure every translatable string within your Portals and Toolkits has a unique string ID.
    - Use Format.JS for consistent string formatting in React components.
    - Create a mapping system in your codebase that associates each string ID with its corresponding translations.

**Managing Translations:**

1. **Initial Translation:**
    - For any new string in the primary language (en_GB), use Amazon Translate to generate translations for all supported languages.
2. **Updating Strings:**
    - When updating strings in the primary language, delete the corresponding translations in other languages and regenerate them using AWS Translate.
    - For non-primary language updates, manually update the strings.

**Quality Assurance:**

1. **Regular Reviews:**
    - Periodically export all new and updated strings to a CSV file and submit it to a professional translation agency for review.
    - Incorporate feedback and corrections from the agency back into your system.

### Supported Languages

**Supported Languages List:**

- Maintain an updated list of all languages supported by your codebase, divided into those supported by React (Format.JS) and PHP.
- Ensure your system can dynamically load the necessary language packs based on the configuration.

### Active Languages

**Configuration:**

1. **Tenant-Level Configuration:**
    - Allow clients to select active languages via a configuration interface.
    - Store this configuration in a database to ensure it’s loaded correctly for each tenant.

### Process

**Language Owners and Managers:**

1. **Language Owners:**
    - Assign a language owner for each supported language. This person is responsible for validating the quality of translations and approving changes.
2. **Overall Language Manager:**
    - Appoint an overall language manager to track which clients have activated which languages. This role is crucial for ensuring accurate billing and service provision.

**Adding Support for a New Language:**

1. **Assignment and Task Creation:**
    - Assign a language owner upon request.
    - Create and assign JIRA tickets for the necessary codebase changes.
2. **Quality Assurance and Deployment:**
    - Ensure all translations go through QA before deployment.
    - Once deployed, update the list of supported languages.

### Updating Existing Language Translations

**String Management:**

1. **Adding New Strings:**
    - Automatically translate new strings from the primary language to all supported languages.
2. **Deleting Strings:**
    - Manually remove deleted primary language strings from all supported languages.
3. **Updating Strings:**
    - For primary language updates, delete and re-translate the affected strings in all supported languages.
    - For non-primary language updates, perform manual updates directly.

### Periodic Review and Professional Translation

- Regularly compile changes into a CSV and submit for professional translation review to ensure accuracy and context appropriateness.

### Adding or Updating Active Languages

**Configuration Changes:**

- Make necessary configuration changes as needed to activate or update languages at the tenant level, ensuring it reflects immediately in the user's experience.

### Summary and Further Reading

- **Documentation:**
    - Maintain comprehensive and up-to-date documentation on supported languages, active languages, and future plans for language support.
    - Ensure the documentation is easily accessible to all team members and stakeholders.

### Conclusion

By implementing this structured approach, you can effectively manage translations on your website, ensuring high quality, consistency, and scalability. Regular reviews and updates, along with a clear assignment of responsibilities, will keep the process smooth and manageable.