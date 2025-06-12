# Project Plan: AegisCloud

**Description:** A simple web hosting platform allowing users to register and manage their domains, built using Ruby on Rails, SQLite3, Tailwind CSS and Devise.


## Development Goals

- [ ] Configure the tailwindcss-rails gem and apply base styles to the application layout.
- [ ] Implement Domain model validations, ensuring name and plan are present and unique within a user's domains.
- [ ] Customize the Domain views (index, show, new, edit) to utilize Tailwind CSS classes for improved aesthetics and responsiveness.
- [ ] Implement authentication logic to associate each Domain with the currently logged-in User. Override the Domains controller to scope queries to the current_user.
- [ ] Modify the Domain controller to prevent users from accessing or modifying domains that do not belong to them. Implement authorization using 'before_action' filters.
- [ ] Add a 'plan' select field to the Domain form, offering predefined hosting plans (e.g., 'Basic', 'Standard', 'Premium'). Define these plans as constants in the Domain model.
- [ ] Implement a status update feature for Domains (e.g., 'Active', 'Inactive', 'Pending'). Allow users to temporarily deactivate their domains.
- [ ] Create a dashboard for users to view their domains, account information, and available plans.
- [ ] Create a basic welcome page to display the current user's email and associated Domains
- [ ] Implement soft deletion of domains. When deleting a domain, instead of actually removing it from the database, set a `deleted_at` timestamp. Filter out soft-deleted domains from regular queries.
