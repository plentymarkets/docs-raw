

# Feedback<a name="feedback_feedback"></a>
    
## Contracts<a name="feedback_feedback_contracts"></a>
### FeedbackAverageRepositoryContract<a name="feedback_contracts_feedbackaveragerepositorycontract"></a>

Get the feedback average.


#### Namespace

`Plenty\Modules\Feedback\Contracts`



#### Methods

<pre>public <strong>getFeedbackAverage</strong>(<a target="_blank" href="http://php.net/int">int</a> $feedbackRelationTargetId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Gets the feedback average
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$feedbackRelationTargetId</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
<pre>public <strong>setFilters</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Sets the filter array.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the filter array.
    
<pre>public <strong>getConditions</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns a collection of parsed filters as Condition object
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    

### FeedbackCommentRepositoryContract<a name="feedback_contracts_feedbackcommentrepositorycontract"></a>

Get, create and delete feedback comments.


#### Namespace

`Plenty\Modules\Feedback\Contracts`



#### Methods

<pre>public <strong>getFeedbackComment</strong>(<a target="_blank" href="http://php.net/int">int</a> $feedbackCommentId):<a href="feedback#feedback_models_feedbackcomment">FeedbackComment</a>
</pre>

    
Get a feedback comment
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$feedbackCommentId</td>
        <td>The ID of the feedback comment</td>
    </tr>
</table>


<pre>public <strong>listFeedbackComments</strong>():<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    
List feedback comments
    
<pre>public <strong>createFeedbackComment</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="feedback#feedback_models_feedbackcomment">FeedbackComment</a>
</pre>

    
Create a feedback comment
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>deleteFeedbackComment</strong>(<a target="_blank" href="http://php.net/int">int</a> $feedbackCommentId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a feedback comment
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$feedbackCommentId</td>
        <td>The ID of the feedback comment</td>
    </tr>
</table>


<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
<pre>public <strong>setFilters</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Sets the filter array.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the filter array.
    
<pre>public <strong>getConditions</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns a collection of parsed filters as Condition object
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    

### FeedbackRatingRepositoryContract<a name="feedback_contracts_feedbackratingrepositorycontract"></a>

Get, create and delete feedback ratings.


#### Namespace

`Plenty\Modules\Feedback\Contracts`



#### Methods

<pre>public <strong>getFeedbackRating</strong>(<a target="_blank" href="http://php.net/int">int</a> $feedbackRatingId):<a href="feedback#feedback_models_feedbackrating">FeedbackRating</a>
</pre>

    
Get a feedback rating
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$feedbackRatingId</td>
        <td>The ID of the feedback rating</td>
    </tr>
</table>


<pre>public <strong>listFeedbackRatings</strong>():<a href="miscellaneous#miscellaneous_support_collection">Collection</a>
</pre>

    
List feedback ratings
    
<pre>public <strong>createFeedbackRating</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="feedback#feedback_models_feedbackrating">FeedbackRating</a>
</pre>

    
Create a feedback rating
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>deleteFeedbackRating</strong>(<a target="_blank" href="http://php.net/int">int</a> $feedbackRatingId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a feedback rating
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$feedbackRatingId</td>
        <td>The ID of the feedback rating</td>
    </tr>
</table>


<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
<pre>public <strong>setFilters</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Sets the filter array.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the filter array.
    
<pre>public <strong>getConditions</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns a collection of parsed filters as Condition object
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    

### FeedbackRepositoryContract<a name="feedback_contracts_feedbackrepositorycontract"></a>

Get, create and delete feedbacks.


#### Namespace

`Plenty\Modules\Feedback\Contracts`



#### Methods

<pre>public <strong>getFeedback</strong>(<a target="_blank" href="http://php.net/int">int</a> $feedbackId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Get a feedback
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$feedbackId</td>
        <td>The ID of the feedback</td>
    </tr>
</table>


<pre>public <strong>listFeedbacks</strong>(<a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = [], <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="miscellaneous#miscellaneous_models_paginatedresult">PaginatedResult</a>
</pre>

    

    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>createFeedback</strong>(<a target="_blank" href="http://php.net/array">array</a> $data):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Create a feedback
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>The request data</td>
    </tr>
</table>


<pre>public <strong>deleteFeedback</strong>(<a target="_blank" href="http://php.net/int">int</a> $feedbackId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete a feedback
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$feedbackId</td>
        <td>The ID of the feedback</td>
    </tr>
</table>


<pre>public <strong>updateFeedback</strong>(<a target="_blank" href="http://php.net/array">array</a> $data, <a target="_blank" href="http://php.net/int">int</a> $feedbackId):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update a feedback
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$data</td>
        <td>Request data</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$feedbackId</td>
        <td>The ID of the feedback</td>
    </tr>
</table>


<pre>public <strong>updateFeedbacksVisibility</strong>(<a target="_blank" href="http://php.net/array">array</a> $feedbackIds, <a target="_blank" href="http://php.net/bool">bool</a> $isVisible):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Update the visibility of multiple feedbacks
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$feedbackIds</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/bool">bool</a></td>
        <td>$isVisible</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>deleteFeedbacks</strong>(<a target="_blank" href="http://php.net/string">string</a> $feedbackIds):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Delete multiple feedbacks
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$feedbackIds</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>listFeedbackReplies</strong>(<a target="_blank" href="http://php.net/int">int</a> $feedbackId, <a target="_blank" href="http://php.net/int">int</a> $page = 1, <a target="_blank" href="http://php.net/int">int</a> $itemsPerPage = 50, <a target="_blank" href="http://php.net/array">array</a> $with = [], <a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Lists feedback replies
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$feedbackId</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$page</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$itemsPerPage</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$with</td>
        <td></td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>migrateLegacyFeedbacks</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Migrate legacy feedbacks
    
<pre>public <strong>clearCriteria</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Resets all Criteria filters by creating a new instance of the builder object.
    
<pre>public <strong>applyCriteriaFromFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Applies criteria classes to the current repository.
    
<pre>public <strong>setFilters</strong>(<a target="_blank" href="http://php.net/array">array</a> $filters = []):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Sets the filter array.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/array">array</a></td>
        <td>$filters</td>
        <td></td>
    </tr>
</table>


<pre>public <strong>getFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns the filter array.
    
<pre>public <strong>getConditions</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Returns a collection of parsed filters as Condition object
    
<pre>public <strong>clearFilters</strong>():<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Clears the filter array.
    
## Models<a name="feedback_feedback_models"></a>
### Feedback<a name="feedback_models_feedback"></a>

The feedback model.


#### Namespace

`Plenty\Modules\Feedback\Models`


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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td>The ID of the feedback</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>title</td>
            <td>The title of the feedback</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>authorName</td>
            <td>The name of the feedback's author</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isVisible</td>
            <td>If true, the feedback is visible</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the feedback was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the feedback was last updated</td>
        </tr><tr>
            <td><a href="feedback#feedback_models_feedbacksourcerelation">FeedbackSourceRelation</a>
</td>
            <td>sourceRelation</td>
            <td>The feedback source relation</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### FeedbackAverage<a name="feedback_models_feedbackaverage"></a>

The feedback average model.


#### Namespace

`Plenty\Modules\Feedback\Models`


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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td>The ID of the feedback average</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>feedbackRelationType</td>
            <td>The feedback relation type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>feedbackRelationTargetId</td>
            <td>The feedback relation target ID</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>averageValue</td>
            <td>The average value of the feedback</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ratingsCountTotal</td>
            <td>The total count of ratings for this target</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ratingsCountOf1</td>
            <td>Number of ratings of 1 for this target</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ratingsCountOf2</td>
            <td>Number of ratings of 2 for this target</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ratingsCountOf3</td>
            <td>Number of ratings of 3 for this target</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ratingsCountOf4</td>
            <td>Number of ratings of 4 for this target</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ratingsCountOf5</td>
            <td>Number of ratings of 5 for this target</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the feedback average was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the feedback average was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### FeedbackComment<a name="feedback_models_feedbackcomment"></a>

The feedback comment model.


#### Namespace

`Plenty\Modules\Feedback\Models`


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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td>The ID of the comment</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>message</td>
            <td>The message of the comment</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isVisible</td>
            <td>If true, the comment is visible</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the feedback relation type name was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the feedback relation type name was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### FeedbackCommentSourceRelation<a name="feedback_models_feedbackcommentsourcerelation"></a>

The feedback comment source relation model.


#### Namespace

`Plenty\Modules\Feedback\Models`


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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>commentId</td>
            <td>The ID of the feedback comment</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>commentRelationType</td>
            <td>The relation comment relation type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>commentRelationSourceId</td>
            <td>The relation comment relation source ID</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### FeedbackCommentTargetRelation<a name="feedback_models_feedbackcommenttargetrelation"></a>

The feedback comment target relation model.


#### Namespace

`Plenty\Modules\Feedback\Models`


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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>commentId</td>
            <td>The ID of the feedback comment</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>commentRelationType</td>
            <td>The relation comment relation type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>commentRelationTargetId</td>
            <td>The relation comment relation target ID</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### FeedbackLegacy<a name="feedback_models_feedbacklegacy"></a>

The feedback legacy model.


#### Namespace

`Plenty\Modules\Feedback\Models`


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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>feedbackId</td>
            <td>The ID of the new feedback</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>legacyFeedbackId</td>
            <td>The ID of the legacy feedback</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the legacy feedback was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the legacy feedback was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### FeedbackRating<a name="feedback_models_feedbackrating"></a>

The feedback rating model.


#### Namespace

`Plenty\Modules\Feedback\Models`


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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td>The ID of the rating</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>ratingValue</td>
            <td>The value of the rating</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/bool">bool</a></td>
            <td>isVisible</td>
            <td>If true, the rating is visible</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the feedback rating relation type name was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the feedback rating relation type name was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### FeedbackRatingAverage<a name="feedback_models_feedbackratingaverage"></a>

The feedback rating average model.


#### Namespace

`Plenty\Modules\Feedback\Models`


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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>id</td>
            <td>The ID of the feedback rating average</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>ratingRelationType</td>
            <td>The feedback rating relation type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ratingRelationTargetId</td>
            <td>The feedback rating relation target ID</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/float">float</a></td>
            <td>averageValue</td>
            <td>The average value of the feedback rating</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>averageCount</td>
            <td>The average count of the feedback rating</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>createdAt</td>
            <td>The date when the feedback rating average was created</td>
        </tr><tr>
            <td><a href="miscellaneous#miscellaneous__"></a>
</td>
            <td>updatedAt</td>
            <td>The date when the feedback rating average was last updated</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### FeedbackRatingSourceRelation<a name="feedback_models_feedbackratingsourcerelation"></a>

The feedback rating source relation model.


#### Namespace

`Plenty\Modules\Feedback\Models`


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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ratingId</td>
            <td>The ID of the feedback rating</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>ratingRelationType</td>
            <td>The rating relation type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ratingRelationSourceId</td>
            <td>The rating relation source ID</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### FeedbackRatingTargetRelation<a name="feedback_models_feedbackratingtargetrelation"></a>

The feedback rating target relation model.


#### Namespace

`Plenty\Modules\Feedback\Models`


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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ratingId</td>
            <td>The ID of the feedback rating</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>ratingRelationType</td>
            <td>The relation rating relation type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>ratingRelationTargetId</td>
            <td>The relation rating relation target ID</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### FeedbackSourceRelation<a name="feedback_models_feedbacksourcerelation"></a>

The feedback source relation model.


#### Namespace

`Plenty\Modules\Feedback\Models`


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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>feedbackId</td>
            <td>The ID of the feedback</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>feedbackRelationType</td>
            <td>The relation type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>feedbackRelationSourceId</td>
            <td>The relation source ID</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sourceRelationLabel</td>
            <td>The source relation label</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>sourceRelationTypeLabel</td>
            <td>The source relation type label</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    

### FeedbackTargetRelation<a name="feedback_models_feedbacktargetrelation"></a>

The feedback target relation model.


#### Namespace

`Plenty\Modules\Feedback\Models`


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
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>feedbackId</td>
            <td>The ID of the feedback</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>feedbackRelationType</td>
            <td>The relation type</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/int">int</a></td>
            <td>feedbackRelationSourceId</td>
            <td>The relation source ID</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>targetRelationLabel</td>
            <td>The target relation label</td>
        </tr><tr>
            <td><a target="_blank" href="http://php.net/string">string</a></td>
            <td>targetRelationName</td>
            <td>The target relation name</td>
        </tr></tbody>
</table>


#### Methods

<pre>public <strong>toArray</strong>()</pre>

    
Returns this model as an array.
    
