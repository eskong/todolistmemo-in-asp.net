# todolistmemo-in-asp.net
<h3>In this sample, will show you</h3>
<ul>
<li>
    <b>Do the memo list </b>
        This example allow you to do memo task that 
        you can create DatabaseInitializer which is configured to get called each time the app starts.
        <strong>Please look in Global.asax and App_Start\IdentityConfig.cs</strong>
        This code shows the following
        <ul>
            <li>Create user</li>
            <li>Create user with password</li>
            <li>Create Roles</li>
            <li>Add Users to Roles</li>
        </ul>
</li>
<li>
    <b>Add profile data for the user</b>
                <ul>
                    <li>Add profile information in the Users Table</li>
                    <li>Add profile information in a different table</li>
                    <li>Look in Models\AppModel.cs for examples</li>
                </ul>
</li>
<li>
    <b>Display profile data for the user</b>
        Click Profile view profile info for the logged in user.
        For the code look in <strong>HomeController.cs Profile Action</strong>

</li>
<li>
       <b>Validation</b>
             When you create a User using a username or password, the Identity system performs validation on the username and password, and the passwords are hashed before they are
                stored in the database. You can customize the validation by changing some of the properties of the validators such as Turn alphanumeric on/off, set minimum password length
                or you can write your own custom validators and register them with the Manager. You can use the same approach for UserManager and RoleManager.
                <ul>
                    <li>Look at Controllers\ValidationController.cs Default Action on how to tweak the default settings for the Validators</li>
                    <li>Look at IdentityExtensibility\MyValidation.cs to see how you can implement the different validators</li>
                    <li>Look at Controllers\ValidationController.cs Cutomize Action on how you can use the custom validators with the Managers</li>
                </ul>

</li>
<li>
    <b>Register a user, Login</b>
    Click Register and see the code in AccountController.cs and Register Action.
        Click Login and see the code in AccountController.cs and Login Action.
</li>
<li>
    <b>Basic Role Management</b>
    Do Create, Update, List and Delete Roles.
        Only Users In Role Admin can access this page. This uses the [Authorize] on the controller.
</li>
<li>
    <b>Basic User Management</b>
        Do Create, Update, List and Delete Users.
        Assign a Role to a User.
        Only Users In Role Admin can access this page. This uses the [Authorize] on the controller.
</li>
<li>
    <b>Associating ToDoes with User</b>
        This example shows how you can create a ToDo application where you can associate ToDoes with a User.
        Following are the salient features of this sample.
        <ul>
            <li>Create ToDo model and associate User in EF Code First. Goto Models\AppModel.cs </li>
            <li>Only Authenticated Users can Create ToDo</li>
            <li>When you create/list ToDo, we can filter by User. Look at ToDoController</li>
            <li>Only Users in Role Admin can see all ToDoes. Look at ToDoController and All action.</li>
        </ul>
</li>
<ul>

