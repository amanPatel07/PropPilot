1. Product Overview

This is a multi-tenant apartment management SaaS application.

It allows:

Platform Admin to manage Super Admin accounts.

Super Admins to manage multiple apartments.

Admins to manage flats, rent, electricity, maintenance.

Tenants to view rent and electricity records (view-only).

Target Users:
Non-tech-savvy apartment managers and tenants.

The application is mobile-first and installable as a PWA.

2. Roles

Platform Admin
Super Admin
Admin
Tenant

Strict role-based access must be enforced via Supabase RLS.

3. Architecture Rules

Multi-tenant architecture

Every data table must include:

super_admin_id

apartment_id (where applicable)

Soft delete required (is_deleted, deleted_at)

No direct Supabase calls inside components

All API communication via RTK Query

4. UI Rules

Mobile-first

Minimalistic design

Large touch-friendly buttons

Clear non-technical labels

No heavy charts in MVP

Hindi, Gujarati, English supported

5. MVP Scope

Included:

Apartment creation

Admin assignment

Flat management

Tenant assignment

Rent entry

Electricity entry

Maintenance tracking

In-app reminders

Excluded:

Payment gateway

Email/WhatsApp notifications

Subscription system

Reports

Public signup

This ensures AI consistency.
