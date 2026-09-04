# CMPUT 301 Project – Syzygy

An Android event management application that allows users to discover events,
join waiting lists, receive invitations, and manage their profiles. Organizers
can create and manage events, while administrators can manage users and events.

## Team Members

* Maheen Abbasi
* Aliha Ali
* Sarah Mohammed
* Alex Kumpula
* Wren Durbano
* Travis Born

## Features

### User

* Create and manage a user profile
* View and update profile information
* Search and filter available events
* View event details
* Join and leave event waiting lists
* View joined events
* Receive and respond to event invitations
* Scan QR codes
* View event locations

### Organizer

* Create events
* Edit existing events
* Delete events
* Manage event information
* View events they organize
* Manage event waiting lists
* Send invitations to users

### Administrator

* Manage users
* View user information
* Change user roles
* Manage events
* Access administrator functionality

## Technologies Used

* Java
* Android
* Firebase Firestore
* Android Camera/QR scanning
* Material Design components

## Project Structure

```text
MainActivity.java                  # Application entry point and main navigation
NavigationStackFragment.java       # Handles fragment navigation and screen stack

User.java                          # Base user entity
Organizer.java                     # Organizer user entity
Admin.java                         # Administrator user entity
Event.java                         # Event entity
Invitation.java                    # Event invitation entity

UserController.java                # User creation and management
EventController.java               # Event creation and management
OrganizerController.java            # Organizer functionality
InvitationController.java           # Invitation management
NotificationController.java        # Notification functionality

ProfileFragment.java               # User profile
FindEventsFragment.java             # Event discovery and search
EventListFragment.java              # Displays lists of events
EventFragment.java                 # Displays event details
JoinedEventsFragment.java           # Displays joined events
QRScanFragment.java                # QR code scanning

OrganizerFragment.java              # Organizer event management
OrganizerEventEditDetailsFragment.java # Create/edit event details
AdministratorFragment.java          # Administrator functionality

EventListAdapter.java              # Displays events in a RecyclerView
UserListView.java                   # Displays users
UserListViewAdapter.java            # User list adapter
EventSummaryView.java               # Event summary component
