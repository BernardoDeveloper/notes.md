Need create a point to register a employee and a enterprise, need create a endpoint to link enterprise with employees

Endpoints to create the system:
**POST** - */user/enterprise*
```json
{
	"name": "name_test",
	"password": "encrypted_password",
	"use_protheus": true
}
```

**POST** - */user/employee*
```json
{
	"name": "name_test",
	"password": "encrypted_password"
}
```

**PUT** - */enterprise/{enterprise_id}*
```json
{
	"employee_name": ["name_test", "name_test_2"]
}
```
