# **Automobile Insurance Claim and Risk Assessment System**

# **📌 Project Overview**
  The Automobile Insurance Claim and Risk Assessment System is a comprehensive web platform designed to streamline car insurance claims and automate policy-based compensation evaluation.

  The system bridges the gap between Insurers (Policyholders) and the Insurance Company (Admins & Staff). It simplifies claim submissions for users while providing company staff with automated tools to assess risk levels, verify claims, calculate compensation based on policy rules, and update claim statuses in real time.

# **💡 Key Workflow & Architecture**
**Claim Submission**: Policyholders submit a claim via the New Claim Module by providing accident details including the date, location, and description.

**Verification**: Upon receiving the claim, company staff contact the policyholder using their registered phone number and conduct on-site or remote verification.

**Assessment & Automated Calculation**: If the claim information is valid, staff initiate processing through the Claims Module. The system evaluates the claim against company rules, considering the policyholder's age, purchased policy limits, and risk factors (e.g., applying specific deductibles/discounts for Medium Risk levels).

**Compensation Calculation**: Calculates whether the requested amount can be fully awarded based on policy coverage limits.

**Risk Assessment**: Re-evaluates and updates the remaining policy coverage limit for future claims.

**Status Updates**: Once submitted by staff, the data is stored in the database, and the user's dashboard updates instantly with the latest claim status. (Note: Direct cash payout operations are handled offline and outside the scope of this system).

# **🛡️ Business Rules & Constraints**
**Policy Coverage Restriction**: Users can only file claims for coverage types explicitly included in their active insurance policy.

**Duplicate Claim Prevention**: Once a claim has been submitted for a specific coverage type under a policy, duplicate claims for that same coverage are blocked.

**5-Day Submission Limit**: Claims must be submitted within 5 calendar days from the date of the accident.

**Data Integrity & Validation**: Strictly enforced required fields, format validations, and duplicate checks across both User and Admin modules.

# **📱 Modules Breakdown**
# **👤 User Side**
**Authentication**: Secure Login and Edit/Change Password functionality.

**Dashboard**: Overview of recent activity.

**New Claim**: Guided claim submission form with strict validation and business rules.

**My Claims**: History list of submitted claims with live status updates (e.g., Pending, Approved, Rejected).

**Profile**: View user information, active policy details, and account settings.

# **🔑 Admin & Staff Side**
**Authentication**: Role-based access control (Admin vs. Staff).

**Dashboard**: System-wide statistics and claim overview analytics.

**Claims Module**: Centralized workspace to view incoming claims, perform risk assessment, compute compensation, and approve/reject claims.

**Coverage Module**: Manage insurance plans offered by the company (includes duplicate checks and field validations).

**Users Module**: Management of registered users, their personal data, and purchased policy histories.

**Staffs Module**: Administrative control for managing staff accounts (Accessible by Admin only).

**Profile**: Management of administrative user profile and security credentials.
