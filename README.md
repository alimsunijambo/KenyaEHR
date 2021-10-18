# KenyaEHR
An open source Electronic Health Record(EHR) customized for Kenyanl’s public healthcare system. It is designed for use in limited resource settings, and seamlessly integrates registration, clinical diagnosis and investigations, prescriptions, reporting, and supply chain management. It facilitates care coordination across facility- and community-based points of service, integrating data to map disease, target care &amp; continuously improve healthcare service delivery.
It integrate implementation of Bahmni open source electronic health record system with OpenERP, Commcare mobile platform, and DHIS2 data visualization platform that allows for digital storage, secure access, maintenance of individual patient’s medical records, supply chain management, and quality improvement - simple enough to be used by mid-level practitioners and community health workers but complex enough to meet demanding population health needs.


 "config" : {
    "otherInvestigationsMap": {
        "Radiology": "Radiology Order",
        "Endoscopy": "Endoscopy Order"
    },
    "conceptSetUI": {   // all configs for conceptSet added here
        "XCodedConcept": {  // name of the concept
            "autocomplete": true,  // if set to true, it will show autocomplete instead of dropdown for coded concept answers.
            "showAbnormalIndicator": true   //If set to true, will show a checkbox for capturing abnormal observation.
        },
        "Text Complaints": {    //name of the concept
            "freeTextAutocomplete": {   //if present, will show a textbox, with autocomplete for concept name.
                "conceptSetName": "VITALS_CONCEPT",  // autocomplete will search for concepts which are membersOf this conceptSet (Optional)
                "codedConceptName": "Complaints"     // autocomplete will search for concepts which are answersTo this codedConcept (Optional)
            }
        }
    }
}

