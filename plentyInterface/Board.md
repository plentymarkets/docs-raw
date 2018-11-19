

# Board<a name="board_board"></a>
    
## Contracts<a name="board_board_contracts"></a>
### BoardColumnRepositoryContract<a name="board_contracts_boardcolumnrepositorycontract"></a>

This interface provides methods to access, create, update or delete columns


#### Namespace

`Plenty\Modules\Board\Contracts`





#### Methods

<pre>public <strong>list</strong>(<a target="_blank" href="http://php.net/string">string</a> $boardId):<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    
Lists all columns assigned to a specific board.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boardId</td>
        <td>The ID of the board to get columns for.</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/string">string</a> $boardId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="board#board_models_boardcolumn">BoardColumn</a>
</pre>

    
Creates a new column and assign it to a specific board.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boardId</td>
        <td>The ID of the board to assign the new column to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>Data of the new column</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/string">string</a> $boardId, <a target="_blank" href="http://php.net/string">string</a> $columnId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="board#board_models_boardcolumn">BoardColumn</a>
</pre>

    
Updates a specific column.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boardId</td>
        <td>The ID of the board where the column belongs to</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$columnId</td>
        <td>The ID of the column to update</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The data to assign to the specified column</td>
    </tr>
</table>


<pre>public <strong>copy</strong>(<a target="_blank" href="http://php.net/string">string</a> $boardId, <a target="_blank" href="http://php.net/string">string</a> $columnId):<a href="board#board_models_boardcolumn">BoardColumn</a>
</pre>

    
Copy a column and all its tasks.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boardId</td>
        <td>The ID of the board where the column belongs to</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$columnId</td>
        <td>The ID of the column to be copied</td>
    </tr>
</table>


<pre>public <strong>updatePosition</strong>(<a target="_blank" href="http://php.net/string">string</a> $boardId, <a target="_blank" href="http://php.net/string">string</a> $columnId, <a target="_blank" href="http://php.net/int">int</a> $newPosition):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Updates the position of a specified column.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boardId</td>
        <td>The ID of the board where the column belongs to</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$columnId</td>
        <td>The ID of the column to update the position for</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$newPosition</td>
        <td>The new position</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/string">string</a> $boardId, <a target="_blank" href="http://php.net/string">string</a> $columnId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes a specific column.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boardId</td>
        <td>The ID of the board where the column belongs to</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$columnId</td>
        <td>The ID of the column to delete</td>
    </tr>
</table>



### BoardTaskRepositoryContract<a name="board_contracts_boardtaskrepositorycontract"></a>

This interface provides methods to access, create, update or delete tasks


#### Namespace

`Plenty\Modules\Board\Contracts`





#### Methods

<pre>public <strong>list</strong>(<a target="_blank" href="http://php.net/string">string</a> $columnId, <a target="_blank" href="http://php.net/int">int</a> $startAt, <a target="_blank" href="http://php.net/int">int</a> $tasksPerPage = 20, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</pre>

    
Lists tasks for a specific column.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$columnId</td>
        <td>The ID of the column to get tasks for</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$startAt</td>
        <td>The position of a task to start listing at</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$tasksPerPage</td>
        <td>Number of tasks to get per page</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>Fields to load for each task</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/string">string</a> $boardId, <a target="_blank" href="http://php.net/string">string</a> $columnId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="board#board_models_boardtask">BoardTask</a>
</pre>

    
Creates a new task and assign it to a specified column.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boardId</td>
        <td>The ID of the board the column belongs to</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$columnId</td>
        <td>The ID of the column to assign the created task to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>Data of the new task</td>
    </tr>
</table>


<pre>public <strong>copy</strong>(<a target="_blank" href="http://php.net/string">string</a> $boardId, <a target="_blank" href="http://php.net/string">string</a> $columnId, <a target="_blank" href="http://php.net/string">string</a> $taskId):<a href="board#board_models_boardtask">BoardTask</a>
</pre>

    
Copies the task with all references.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boardId</td>
        <td>The ID of the board the column belongs to</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$columnId</td>
        <td>The ID of the column to assign the copied task to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$taskId</td>
        <td>The ID of the task to be copied</td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $taskId):<a href="board#board_models_boardtask">BoardTask</a>
</pre>

    
Returns a task for a given ID.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$taskId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/string">string</a> $boardId, <a target="_blank" href="http://php.net/string">string</a> $columnId, <a target="_blank" href="http://php.net/string">string</a> $taskId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="board#board_models_boardtask">BoardTask</a>
</pre>

    
Updates a specified task.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boardId</td>
        <td>The ID of the board the column belongs to</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$columnId</td>
        <td>The ID of the column the task belongs to.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$taskId</td>
        <td>The ID of the task to update</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>Data to set at the task</td>
    </tr>
</table>


<pre>public <strong>addReference</strong>(<a href="board#board_models_boardtaskreference">BoardTaskReference</a>
 $boardTaskReference):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Add task reference to task object
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="board#board_models_boardtaskreference">BoardTaskReference</a>
</td>
        <td>$boardTaskReference</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>removeReference</strong>(<a href="board#board_models_boardtaskreference">BoardTaskReference</a>
 $boardTaskReference):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Remove task reference from task object
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a href="board#board_models_boardtaskreference">BoardTaskReference</a>
</td>
        <td>$boardTaskReference</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>updatePosition</strong>(<a target="_blank" href="http://php.net/string">string</a> $taskId, <a target="_blank" href="http://php.net/string">string</a> $newColumnId, <a target="_blank" href="http://php.net/int">int</a> $newPosition):<a target="_blank" href="http://php.net/int">int</a></pre>

    
Updates the position of a specified task.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$taskId</td>
        <td>The ID of the task to update the position for</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$newColumnId</td>
        <td>The ID of the column the task now belongs to</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$newPosition</td>
        <td>The new position</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/string">string</a> $taskId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes a specified task.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$taskId</td>
        <td>The ID of the task to delete</td>
    </tr>
</table>


<pre>public <strong>deleteByColumn</strong>(<a target="_blank" href="http://php.net/string">string</a> $boardId, <a target="_blank" href="http://php.net/string">string</a> $columnId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes all tasks of a column
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boardId</td>
        <td>The ID of the board where the column belongs to</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$columnId</td>
        <td>The ID of the column where the task belongs to</td>
    </tr>
</table>


<pre>public <strong>allByColumnId</strong>(<a target="_blank" href="http://php.net/string">string</a> $columnId, <a target="_blank" href="http://php.net/string">string</a> $referenceValue = null, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get all tasks for the given column id having a reference with the given reference value.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$columnId</td>
        <td>The column id of the tasks</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$referenceValue</td>
        <td>The reference value that has to be contained in the task. Can be NULL.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The attributes of the task to load.</td>
    </tr>
</table>


<pre>public <strong>allByBoardId</strong>(<a target="_blank" href="http://php.net/string">string</a> $boardId, <a target="_blank" href="http://php.net/string">string</a> $referenceValue = null, <a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get all tasks for the given column id having a reference with the given reference value.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boardId</td>
        <td>The board id of the tasks</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$referenceValue</td>
        <td>The reference value that has to be contained in the task. Can be NULL.</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>The attributes of the task to load.</td>
    </tr>
</table>



### BoardRepositoryContract<a name="board_contracts_boardrepositorycontract"></a>

This interface provides all methods to access, create, update or delete boards.


#### Namespace

`Plenty\Modules\Board\Contracts`





#### Methods

<pre>public <strong>list</strong>(<a target="_blank" href="http://php.net/array">array</a> $columns = []):<a href="miscellaneous#miscellaneous_eloquent_collection">Collection</a>
</pre>

    
List all boards.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$columns</td>
        <td>Fields to load for each board</td>
    </tr>
</table>


<pre>public <strong>get</strong>(<a target="_blank" href="http://php.net/string">string</a> $boardId, <a target="_blank" href="http://php.net/int">int</a> $tasksPerPage = 20):<a href="board#board_models_board">Board</a>
</pre>

    
Returns a single board.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boardId</td>
        <td>The ID of the board to get</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$tasksPerPage</td>
        <td>Maximum number of tasks to load for each column</td>
    </tr>
</table>


<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="board#board_models_board">Board</a>
</pre>

    
Creates a new board.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>Data of the new board</td>
    </tr>
</table>


<pre>public <strong>update</strong>(<a target="_blank" href="http://php.net/string">string</a> $boardId, <a target="_blank" href="http://php.net/array">array</a> $data):<a href="board#board_models_board">Board</a>
</pre>

    
Updates a board.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boardId</td>
        <td>The ID of the board to be updated</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>New data to be assigned to the board if exists</td>
    </tr>
</table>


<pre>public <strong>copy</strong>(<a target="_blank" href="http://php.net/string">string</a> $boardId):<a href="board#board_models_board">Board</a>
</pre>

    
Copy a board and all its columns.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boardId</td>
        <td>The ID of the board to be copied</td>
    </tr>
</table>


<pre>public <strong>updateTasksCount</strong>(<a target="_blank" href="http://php.net/string">string</a> $boardId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Update tasks count value
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boardId</td>
        <td>The ID of the board to update the tasks count</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/string">string</a> $boardId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes a board. Returns `true` if the deletion was successful.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$boardId</td>
        <td>The ID of the board to delete</td>
    </tr>
</table>



### BoardTaskReferenceRepositoryContract<a name="board_contracts_boardtaskreferencerepositorycontract"></a>

This interface provides methods to create or delete references from tasks to contacts or tickets


#### Namespace

`Plenty\Modules\Board\Contracts`





#### Methods

<pre>public <strong>create</strong>(<a target="_blank" href="http://php.net/string">string</a> $taskId, <a target="_blank" href="http://php.net/string">string</a> $referenceValue):<a href="board#board_models_boardtaskreference">BoardTaskReference</a>
</pre>

    
Creates a new reference to a given task.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$taskId</td>
        <td>The ID of the task to create a reference for</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$referenceValue</td>
        <td>Reference type followed by foreign ID of the referenced object. Syntax: TYPE-ID Example: user-123456 Types: user,ticket,contact,order,item</td>
    </tr>
</table>


<pre>public <strong>delete</strong>(<a target="_blank" href="http://php.net/string">string</a> $referenceId):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Deletes a specific reference.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$referenceId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>checkReferenceKey</strong>(<a target="_blank" href="http://php.net/string">string</a> $referenceType, <a target="_blank" href="http://php.net/int">int</a> $referenceKey):<a target="_blank" href="http://php.net/bool">bool</a></pre>

    
Check whether the reference key for the given reference type exists or not.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$referenceType</td>
        <td>The reference type (one of 'contact', 'order', 'item', 'ticket' or 'user')</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$referenceKey</td>
        <td>The ID of the correspnding reference type</td>
    </tr>
</table>


## Models<a name="board_board_models"></a>
### BoardTaskReference<a name="board_models_boardtaskreference"></a>

The task reference model.


#### Namespace

`Plenty\Modules\Board\Models`




#### Properties

<table class="table table-bordered table-striped table-condensed table-hover">
    <thead>
    <tr>
        <th>Type</th>
        <th>Name</th>
        <th>Description</th>
    </tr>
    </thead>
    <tbody><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>taskId</td>
            <td>The ID of the task to create a reference for</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>referenceValue</td>
            <td>Reference type followed by foreign ID of the referenced object. Syntax: TYPE-ID Example: user-123456 Types: user,ticket,contact,order,item</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### Board<a name="board_models_board"></a>

the board model.


#### Namespace

`Plenty\Modules\Board\Models`




#### Properties

<table class="table table-bordered table-striped table-condensed table-hover">
    <thead>
    <tr>
        <th>Type</th>
        <th>Name</th>
        <th>Description</th>
    </tr>
    </thead>
    <tbody><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>boardName</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</td>
            <td>boardColumns</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>columnsCount</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>tasksCount</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### BoardColumn<a name="board_models_boardcolumn"></a>

the board column model.


#### Namespace

`Plenty\Modules\Board\Models`




#### Properties

<table class="table table-bordered table-striped table-condensed table-hover">
    <thead>
    <tr>
        <th>Type</th>
        <th>Name</th>
        <th>Description</th>
    </tr>
    </thead>
    <tbody><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>boardId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>columnName</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>tasks</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### BoardTask<a name="board_models_boardtask"></a>

the board task model.


#### Namespace

`Plenty\Modules\Board\Models`




#### Properties

<table class="table table-bordered table-striped table-condensed table-hover">
    <thead>
    <tr>
        <th>Type</th>
        <th>Name</th>
        <th>Description</th>
    </tr>
    </thead>
    <tbody><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>id</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>taskName</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>description</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>position</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>columnId</td>
            <td></td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>boardId</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>tags</td>
            <td></td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>references</td>
            <td></td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
## Events<a name="board_board_events"></a>
### AfterBoardTaskReferenceCreated<a name="board_events_afterboardtaskreferencecreated"></a>

This event will be triggered, after a task reference was created.


#### Namespace

`Plenty\Modules\Board\Events`





#### Methods

<pre>public <strong>getBoardTaskReference</strong>():<a href="board#board_models_boardtaskreference">BoardTaskReference</a>
</pre>

    

    

### BeforeBoardColumnDeleted<a name="board_events_beforeboardcolumndeleted"></a>

This event will be triggered, before a board column will be deleted.


#### Namespace

`Plenty\Modules\Board\Events`





#### Methods

<pre>public <strong>getBoard</strong>():<a href="board#board_models_board">Board</a>
</pre>

    

    
<pre>public <strong>getColumnId</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    

### AfterBoardTaskDeleted<a name="board_events_afterboardtaskdeleted"></a>

This event will be triggered, when a single board task was deleted. It won&#039;t be triggered, if a board column was deleted.


#### Namespace

`Plenty\Modules\Board\Events`





#### Methods

<pre>public <strong>getBoardTask</strong>():<a href="board#board_models_boardtask">BoardTask</a>
</pre>

    

    

### AfterBoardColumnTasksDeleted<a name="board_events_afterboardcolumntasksdeleted"></a>

This event will be triggered, after all tasks of a column were deleted.


#### Namespace

`Plenty\Modules\Board\Events`





#### Methods

<pre>public <strong>getBoardId</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getColumnId</strong>():<a target="_blank" href="http://php.net/string">string</a></pre>

    

    
<pre>public <strong>getDeletedTaskIdList</strong>():<a target="_blank" href="http://php.net/array">array</a></pre>

    

    

### BeforeBoardDeleted<a name="board_events_beforeboarddeleted"></a>

This event will be triggered, before a board will be deleted.


#### Namespace

`Plenty\Modules\Board\Events`





#### Methods

<pre>public <strong>getBoard</strong>():<a href="board#board_models_board">Board</a>
</pre>

    

    

### AfterBoardTaskReferenceDeleted<a name="board_events_afterboardtaskreferencedeleted"></a>

This event will be triggered, after a task reference was deleted.


#### Namespace

`Plenty\Modules\Board\Events`





#### Methods

<pre>public <strong>getBoardTaskReference</strong>():<a href="board#board_models_boardtaskreference">BoardTaskReference</a>
</pre>

    

    

### AfterBoardTaskCreated<a name="board_events_afterboardtaskcreated"></a>

This event will be triggered, when a board task was created.


#### Namespace

`Plenty\Modules\Board\Events`





#### Methods

<pre>public <strong>getBoardTask</strong>():<a href="board#board_models_boardtask">BoardTask</a>
</pre>

    

    

### BeforeBoardTaskDeleted<a name="board_events_beforeboardtaskdeleted"></a>

This event will be triggered, before a single board task was deleted. It won&#039;t be triggered, if a board column will be deleted.


#### Namespace

`Plenty\Modules\Board\Events`





#### Methods

<pre>public <strong>getBoardTask</strong>():<a href="board#board_models_boardtask">BoardTask</a>
</pre>

    

    
