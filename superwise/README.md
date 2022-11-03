# Superwise Integration

## Overview
[Superwise][1] provides model observability for high-scale machine learning (ML) operations.
Superwise's model observability gives you visibility and context into your models' behaviors, so you can easily monitor model risks based on different use cases. With Superwise, data scientists, ML engineers, and business ops get model observability without alert fatigue, so you can be confident about your model management.

![Superwise Dashboard][2]

Superwise's model metrics and incidents integration sends out-of-the-box model metrics, including drift, activity, incidents, and custom metrics, directly to Datadog. You get an overview of which models are not predicting the expected results, which can be configured to any use case, logic, segmentation, threshold, and sensitivity.

With the Datadog integration configured in Superwise, standard model metrics are sent to Datadog, and users get model observability dashboards in Datadog. You can configure any specific model metric and incident policy, and send them to Datadog for model observability that is tailored to your use case.

## Setup

1. Go to [Superwise portal][3] and select **Integrations**.

2. Click **Create a new channel** and select **Datadog**.

    ![Superwise - Add new integration][4]

3. Input your Datadog API and application keys, and click **Test**. A test request is sent to your Datadog account to validate the integration. If the request was successfully sent, there is a message in Superwise saying the test was delivered successfully. To finish the setup, click **Create channel**.

    ![Superwise - Add new Datadog channel][5]

4. When setup is complete, the new Datadog integration widget is available:

    ![Superwise Integration][6]

### Validation
In Datadog, go to **Metrics Explorer** and search for the metric `superwise.integration.test` to verify that the integration between Superwise and Datadog is working.

![superwise.integration.test graph in Datadog][7]

## Data Collected

### Metrics

See [metadata.csv][8] for a list of metrics provided by this check.

### Events

The Superwise integration does not include any events.

### Service Checks

The Superwise integration does not include any service checks.

## Troubleshooting

Need help? See the [Superwise documentation][9].

## Further Reading

Additional helpful documentation, links, and articles:

- [Monitor model performance with Superwise's offering in the Datadog Marketplace][10]

[1]: https://www.superwise.ai/
[2]: https://raw.githubusercontent.com/DataDog/integrations-extras/master/superwise/images/5.png
[3]: https://portal.superwise.ai/
[4]: https://raw.githubusercontent.com/DataDog/integrations-extras/master/superwise/images/2.png
[5]: https://raw.githubusercontent.com/DataDog/integrations-extras/master/superwise/images/6.png
[6]: https://raw.githubusercontent.com/DataDog/integrations-extras/master/superwise/images/3.png
[7]: https://raw.githubusercontent.com/DataDog/integrations-extras/master/superwise/images/4.png
[8]: https://github.com/DataDog/integrations-extras/blob/master/superwise/metadata.csv
[9]: https://docs.superwise.ai
[10]: https://www.datadoghq.com/blog/superwise-datadog-marketplace/
