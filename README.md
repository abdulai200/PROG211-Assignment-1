# PROG211-Assignment-1
Digital  Permit System 
Digital Permit & License Management System

PROG211 Object-Oriented Programming 1 – Government domain Limkokwing University of Creative Technology, Sierra Leone

A simple Python program that lets citizens apply for permits and licenses, and lets officers approve, renew or revoke them.

How to run
python permit_system.py

Choose 1 for the automatic demo or 2 for the interactive menu. Requires Python 3.8+ and no extra libraries.

OOP concepts used
Requirement	Where
Two+ classes	Citizen, Permit, PermitRegistry
Attributes	citizen_code, nickname, permit_id, status, expiry_date ...
Instance methods	approve(), renew(), revoke(), display_info(), apply_for_permit()
Class methods	Permit.total_permits(), Permit.from_application(), Citizen._next_code()
Static method	Permit.is_valid_type()
One data structure	A dictionary in PermitRegistry, keyed by permit ID
Tuple (optional)	PERMIT_TYPES constant
Object interaction	Citizen.apply_for_permit() creates a Permit and adds it to the registry
DPG alignment
Open-source: all code is public on GitHub, with no proprietary dependencies.
Inclusive and accessible: text-only menu, plain-language messages, no reliance on colour, works on low-spec devices.
Privacy-respecting: citizens are identified only by an anonymous code (e.g. CIT-001). No national ID, full name, address or phone number is stored.
Modular and reusable: each class has a single responsibility; Permit and PermitRegistry can be reused for other licence types.
Sample output
Aminata (CIT-001) applied for Business License. Reference: PRM-0001
PRM-0001 approved. Expires 2027-10-28.
PRM-0002 | Market Trading Permit | Holder: CIT-002 | Status: Active | Expires: 2027-04-24
Total permits created: 3
Error handled: Unknown permit type: Fishing Permit
