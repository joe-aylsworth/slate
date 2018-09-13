# GetAvailablePermissionList

 

Retrieves a comma-separated array of all permissions that can be assigned to a user.

An administrator or superuser can set permissions for each user on an API-call by API-call basis, to allow for highly granular control. Common permission sets include *Trading, Deposit,* and *Withdrawal* (which allow trading, deposit of funds, and account withdrawals, respectively); or *AdminUI, UserOperator,* and *AccountOperator* (which allow control of the Order Management System, set of users, or an account). See [“Permissions” on page 4 ](#_bookmark7)for more information, but a complete discussion of permissions and their scope is beyond this API guide.



### Request

The request for **GetAvailablePermissionList** does not require a UserId. It returns a list of all permissions available.

```
	{ }
```

 

### Response

A successful response returns an alphabetically sorted list of all permissions that can be assigned by an administrator or superuser.

```
	[

		“AccountReadOnly”,
		“AddAccount”,
		“AddBalanceReconciliationInfo”,
		“AddDepositTicketAttachment”,
		“AddEditAccountBadge”,
		“AddEditExchange”,
		“AddEditExchangeInstrument”,
		“AddEditOMS”,
		“AddEditOperatorEmail”,
		“AddInstrument”,
		“AddOperator”,
		“AddOperatorOms”,
	...
	]
```

 



------

######  *See Also*

**GetUserPermissions**

------

 



