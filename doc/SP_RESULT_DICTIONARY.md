
# RESULT DICTIONARY

This document has the purpose of explaining the system stored procedures possible returns.

## Positive Results

Here lies all the possible codes returned by each procedure when it succeeds.

- <b>CU:</b> code returned by `SP_CREATE_USER` when a new user is successfully created;
- <b>SUI:</b> code returned by `SP_SET_USER_INACTIVE` when an user successfully schedule the exclusion of their account;
- <b>CTG:</b> code returned by `SP_CREATE_TASK_GROUP` when a task group is successfully created;
- <b>DTG:</b> code returned by `SP_DELETE_TASK_GROUP` when a task group is successfully deleted;
- <b>CT:</b> code returned by `SP_CREATE_TASK` when a task is successfully created;
- <b>ST:</b> code returned by `SP_SELECT_TASK` when a task is successfully selected;
- <b>DT:</b> code returned by `SP_DELETE_TASK` when a task is successfully deleted;
- <b>CCT:</b> code returned by `SP_CONCLUDE_TASK` when a task is successfully marked as concluded;
- <b>SUA:</b> code returned by `SP_SET_USER_ACTIVE` when an user successfully cancels their account scheduled deletion;
- <b>SAT:</b> code returned by `TELEGRAM_SELECT_ALL_TASKS` script when a user successfully requests more information about a specific group;



## Negative Results

Here lies all the possible codes (exceptions) returned by each procedure when it fails.

### Generics

These codes are returned by more than one procedure.

- <b>GNE-1:</b> the provided `@USER_ID` is invalid;
- <b>GNE-2:</b> the provided `@USER_ID` could not be found in the database;
- <b>GNE-3:</b> unhandled error;
- <b>GNE-4:</b> the provided `@GROUP_ID` is invalid;
- <b>GNE-5:</b> the provided `@TASK_ID` is invalid;
- <b>GNE-6:</b> the provided `@USER_ID` does not have a task with the given `@TASK_ID`;
- <b>GNE-7:</b> the account with the given `@USER_ID` is scheduled to be deleted;

### SP_CREATE_NEW_USER

These codes are returned by `SP_CREATE_NEW_USER` only.

- <b>CU-1:</b> the specified user is already registered in the database;

### SP_SET_USER_INACTIVE

These codes are returned by `SP_SET_USER_INACTIVE` only.

- <b>SUI-1:</b> the specified user already scheduled the deletion of their account;

### SP_CREATE_TASK_GROUP

These codes are returned by `SP_CREATE_TASK_GROUP` only.

- <b>CTG-1:</b> the provided `@GROUP_NAME` is invalid;

### SP_CREATE_TASK

These codes are returned by `SP_CREATE_TASK` only.

- <b>CT-1:</b> the given `@TASK_NAME` is invalid;
- <b>CT-2:</b> user does not have a task group with the given `@GROUP_ID`;

### SP_DELETE_TASK

These codes are returned by `SP_DELETE_TASK` only.

- <b>DT-1:</b> user does not have a task with the given `@TASK_ID`;

### SP_DELETE_TASK_GROUP

These codes are returned by `SP_DELETE_TASK_GROUP` only.

- <b>DTG-1:</b> user does not have a task group with the given `@GROUP_ID`;

### SP_SELECT_TASK_GROUP

These codes are returned by `SP_SELECT_TASK_GROUP` only.

- <b>STF-1:</b> user does not have a task group with the given `@GROUP_ID`;

### SP_SET_USER_ACTIVE

These codes are returned by `SP_SET_USER_ACTIVE` only.

- <b>STF-1:</b> user does not have a scheduled account deletion;

### SP_SELECT_TASK

These codes are returned by `SP_SELECT_TASK` only.

- <b>STF-1:</b> user does not have a task with the given `@TASK_ID`;
