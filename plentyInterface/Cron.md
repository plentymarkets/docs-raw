

# Cron<a name="cron_cron"></a>
    
## Contracts<a name="cron_cron_contracts"></a>
### CronHandler<a name="cron_contracts_cronhandler"></a>

CronHandler interface for extending cron handlers.


#### Namespace

`Plenty\Modules\Cron\Contracts`


## Services<a name="cron_cron_services"></a>
### CronContainer<a name="cron_services_croncontainer"></a>

Register cron jobs


#### Namespace

`Plenty\Modules\Cron\Services`



#### Methods

<pre>public <strong>add</strong>(<a target="_blank" href="http://php.net/int">int</a> $schedule, <a target="_blank" href="http://php.net/string">string</a> $handlerClass):<a href="miscellaneous#miscellaneous__void">void</a>
</pre>

    
Use this method to add a handler class and a schedule time for your desired cron event. The action will then be triggered according to the given schedule.
    
##### <strong>Parameters</strong>
    
<table class="table table-condensed">    <tr>
        <td><a target="_blank" href="http://php.net/int">int</a></td>
        <td>$schedule</td>
        <td>The number of minutes for which the cron action should be scheduled. Currently allowed are: 15, 20, 60 and 3600. You can also use constants like `CronContainer::EVERY_FIFTEEN_MINUTES`, `CronContainer::EVERY_TWENTY_MINUTES`, `CronContainer::HOURLY`, `CronContainer::DAILY`;</td>
    </tr>
    <tr>
        <td><a target="_blank" href="http://php.net/string">string</a></td>
        <td>$handlerClass</td>
        <td>The handler class that should be triggered when the cron event is launched. This class has to extend the CronHandler interface and implement the `handle()` method.</td>
    </tr>
</table>


