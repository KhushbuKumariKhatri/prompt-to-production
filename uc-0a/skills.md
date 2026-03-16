skills:
  - name: classify_complaint
    description: Classifies a citizen complaint into the correct municipal department.
    input: Complaint description text.
    output: Department category and a reason referencing keywords.
    error_handling: If no category can be determined return category "Other" with flag "NEEDS_REVIEW".

  - name: extract_keywords
    description: Extracts important keywords from complaint text.
    input: Complaint description.
    output: List of detected keywords.
    error_handling: If no keywords exist return empty list.
