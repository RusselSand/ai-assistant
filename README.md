Here are logs from Rasa:
2025-05-06 14:46:19 DEBUG    rasa.cli.utils  - Parameter 'credentials' not set. Using default location 'credentials.yml' instead.
/home/lerazyukina/architecture-virtual_assistant/rasa_env/lib/python3.10/site-packages/sanic_cors/extension.py:39: DeprecationWarning: distutils Version classes are deprecated. Use packaging.version instead.
  SANIC_VERSION = LooseVersion(sanic_version)
2025-05-06 14:46:20 DEBUG    h5py._conv  - Creating converter from 7 to 5
2025-05-06 14:46:20 DEBUG    h5py._conv  - Creating converter from 5 to 7
2025-05-06 14:46:20 DEBUG    h5py._conv  - Creating converter from 7 to 5
2025-05-06 14:46:20 DEBUG    h5py._conv  - Creating converter from 5 to 7
2025-05-06 14:46:20 DEBUG    jax._src.path  - etils.epath was not found. Using pathlib for file I/O.
/home/lerazyukina/architecture-virtual_assistant/rasa_env/lib/python3.10/site-packages/tensorflow/lite/python/util.py:52: DeprecationWarning: jax.xla_computation is deprecated. Please use the AOT APIs.
  from jax import xla_computation as _xla_computation
<frozen importlib._bootstrap>:283: DeprecationWarning: the load_module() method is deprecated and slated for removal in Python 3.12; use exec_module() instead
2025-05-06 14:46:22 DEBUG    rasa.core.utils  - Available web server routes: 
/conversations/<conversation_id:path>/messages     POST                           add_message
/conversations/<conversation_id:path>/tracker/events POST                           append_events
/webhooks/rasa                                     GET                            custom_webhook_RasaChatInput.health
/webhooks/rasa/webhook                             POST                           custom_webhook_RasaChatInput.receive
/webhooks/rest                                     GET                            custom_webhook_RestInput.health
/webhooks/rest/webhook                             POST                           custom_webhook_RestInput.receive
/model/test/intents                                POST                           evaluate_intents
/model/test/stories                                POST                           evaluate_stories
/conversations/<conversation_id:path>/execute      POST                           execute_action
/domain                                            GET                            get_domain
/                                                  GET                            hello
/model                                             PUT                            load_model
/model/parse                                       POST                           parse
/conversations/<conversation_id:path>/predict      POST                           predict
/conversations/<conversation_id:path>/tracker/events PUT                            replace_events
/conversations/<conversation_id:path>/story        GET                            retrieve_story
/conversations/<conversation_id:path>/tracker      GET                            retrieve_tracker
/status                                            GET                            status
/model/predict                                     POST                           tracker_predict
/model/train                                       POST                           train
/conversations/<conversation_id:path>/trigger_intent POST                           trigger_intent
/model                                             DELETE                         unload_model
/version                                           GET                            version
2025-05-06 14:46:22 INFO     root  - Starting Rasa server on http://0.0.0.0:5005
2025-05-06 14:46:22 DEBUG    rasa.core.utils  - Using the default number of Sanic workers (1).
/home/lerazyukina/architecture-virtual_assistant/rasa_env/lib/python3.10/site-packages/rasa/shared/core/slot_mappings.py:224: UserWarning: Slot auto-fill has been removed in 3.0 and replaced with a new explicit mechanism to set slots. Please refer to https://rasa.com/docs/rasa/domain#slots to learn more.
  rasa.shared.utils.io.raise_warning(
2025-05-06 14:46:22 DEBUG    rasa.telemetry  - Skipping telemetry reporting: no license hash found.
2025-05-06 14:46:22 DEBUG    rasa.core.tracker_store  - Connected to InMemoryTrackerStore.
2025-05-06 14:46:22 DEBUG    rasa.core.lock_store  - Connected to lock store 'InMemoryLockStore'.
2025-05-06 14:46:22 DEBUG    rasa.core.nlg.generator  - Instantiated NLG to 'TemplatedNaturalLanguageGenerator'.
2025-05-06 14:46:22 INFO     rasa.core.processor  - Loading model models/20250506-143014-warm-seller.tar.gz...
2025-05-06 14:46:22 DEBUG    rasa.engine.storage.local_model_storage  - Extracted model to '/tmp/tmpp2hz_pga'.
2025-05-06 14:46:22 DEBUG    rasa.engine.graph  - Node 'nlu_message_converter' loading 'NLUMessageConverter.load' and kwargs: '{}'.
2025-05-06 14:46:22 DEBUG    rasa.engine.graph  - Node 'run_WhitespaceTokenizer0' loading 'WhitespaceTokenizer.load' and kwargs: '{}'.
2025-05-06 14:46:22 DEBUG    rasa.engine.graph  - Node 'run_RegexFeaturizer1' loading 'RegexFeaturizer.load' and kwargs: '{}'.
2025-05-06 14:46:22 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_RegexFeaturizer1' was requested for reading.
2025-05-06 14:46:22 DEBUG    rasa.engine.graph  - Node 'run_LexicalSyntacticFeaturizer2' loading 'LexicalSyntacticFeaturizer.load' and kwargs: '{}'.
2025-05-06 14:46:22 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_LexicalSyntacticFeaturizer2' was requested for reading.
2025-05-06 14:46:22 DEBUG    rasa.engine.graph  - Node 'run_CountVectorsFeaturizer3' loading 'CountVectorsFeaturizer.load' and kwargs: '{}'.
2025-05-06 14:46:22 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_CountVectorsFeaturizer3' was requested for reading.
2025-05-06 14:46:22 DEBUG    rasa.engine.graph  - Node 'run_LanguageModelFeaturizer4' loading 'LanguageModelFeaturizer.load' and kwargs: '{}'.
2025-05-06 14:46:23 DEBUG    rasa.nlu.featurizers.dense_featurizer.lm_featurizer  - Loading Tokenizer and Model for bert
2025-05-06 14:46:23 DEBUG    urllib3.connectionpool  - Starting new HTTPS connection (1): huggingface.co:443
2025-05-06 14:46:23 DEBUG    urllib3.connectionpool  - https://huggingface.co:443 "HEAD /bert-base-cased/resolve/main/tokenizer_config.json HTTP/1.1" 200 0
2025-05-06 14:46:23 DEBUG    urllib3.connectionpool  - https://huggingface.co:443 "HEAD /bert-base-cased/resolve/main/config.json HTTP/1.1" 200 0
Some weights of the PyTorch model were not used when initializing the TF 2.0 model TFBertModel: ['cls.predictions.transform.dense.bias', 'cls.predictions.transform.dense.weight', 'cls.seq_relationship.weight', 'cls.predictions.bias', 'cls.predictions.transform.LayerNorm.weight', 'cls.predictions.transform.LayerNorm.bias', 'cls.seq_relationship.bias']
- This IS expected if you are initializing TFBertModel from a PyTorch model trained on another task or with another architecture (e.g. initializing a TFBertForSequenceClassification model from a BertForPreTraining model).
- This IS NOT expected if you are initializing TFBertModel from a PyTorch model that you expect to be exactly identical (e.g. initializing a TFBertForSequenceClassification model from a BertForSequenceClassification model).
All the weights of TFBertModel were initialized from the PyTorch model.
If your task is similar to the task the model of the checkpoint was trained on, you can already use TFBertModel for predictions without further training.
2025-05-06 14:46:26 DEBUG    rasa.engine.graph  - Node 'run_DIETClassifier5' loading 'DIETClassifier.load' and kwargs: '{}'.
2025-05-06 14:46:26 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_DIETClassifier5' was requested for reading.
2025-05-06 14:46:26 DEBUG    rasa.utils.tensorflow.models  - Loading the model from /tmp/tmp9tn673df/train_DIETClassifier5/DIETClassifier.tf_model with finetune_mode=False...
2025-05-06 14:46:26 DEBUG    rasa.nlu.classifiers.diet_classifier  - You specified 'DIET' to train entities, but no entities are present in the training data. Skipping training of entities.
2025-05-06 14:46:26 DEBUG    rasa.nlu.classifiers.diet_classifier  - Following metrics will be logged during training: 
2025-05-06 14:46:26 DEBUG    rasa.nlu.classifiers.diet_classifier  -   t_loss (total loss)
2025-05-06 14:46:26 DEBUG    rasa.nlu.classifiers.diet_classifier  -   i_acc (intent acc)
2025-05-06 14:46:26 DEBUG    rasa.nlu.classifiers.diet_classifier  -   i_loss (intent loss)
/usr/lib/python3.10/random.py:370: DeprecationWarning: non-integer arguments to randrange() have been deprecated since Python 3.10 and will be removed in a subsequent version
  return self.randrange(a, b+1)
2025-05-06 14:46:35 DEBUG    rasa.utils.tensorflow.models  - Finished loading the model.
/home/lerazyukina/architecture-virtual_assistant/rasa_env/lib/python3.10/site-packages/rasa/utils/train_utils.py:530: UserWarning: constrain_similarities is set to `False`. It is recommended to set it to `True` when using cross-entropy loss.
  rasa.shared.utils.io.raise_warning(
/home/lerazyukina/architecture-virtual_assistant/rasa_env/lib/python3.10/site-packages/rasa/shared/utils/io.py:100: UserWarning: 'evaluate_every_number_of_epochs=20' is greater than 'epochs=1'. No evaluation will occur.
2025-05-06 14:46:35 DEBUG    rasa.engine.graph  - Node 'run_EntitySynonymMapper6' loading 'EntitySynonymMapper.load' and kwargs: '{}'.
2025-05-06 14:46:35 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_EntitySynonymMapper6' was requested for reading.
2025-05-06 14:46:35 DEBUG    rasa.nlu.extractors.entity_synonyms  - Failed to load ABCMeta from model storage. Resource 'train_EntitySynonymMapper6' doesn't exist.
2025-05-06 14:46:35 DEBUG    rasa.engine.graph  - Node 'run_ResponseSelector7' loading 'ResponseSelector.load' and kwargs: '{}'.
2025-05-06 14:46:35 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_ResponseSelector7' was requested for reading.
2025-05-06 14:46:35 DEBUG    rasa.nlu.classifiers.diet_classifier  - Failed to load ABCMeta from model storage. Resource 'train_ResponseSelector7' doesn't exist.
2025-05-06 14:46:35 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_ResponseSelector7' was requested for reading.
2025-05-06 14:46:35 DEBUG    rasa.nlu.selectors.response_selector  - Failed to load ResponseSelector from model storage. Resource 'train_ResponseSelector7' doesn't exist.
2025-05-06 14:46:35 DEBUG    rasa.engine.graph  - Node 'run_RegexMessageHandler' loading 'RegexMessageHandler.load' and kwargs: '{}'.
2025-05-06 14:46:35 DEBUG    rasa.engine.graph  - Node 'domain_provider' loading 'DomainProvider.load' and kwargs: '{}'.
2025-05-06 14:46:35 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'domain_provider' was requested for reading.
<frozen importlib._bootstrap>:283: DeprecationWarning: the load_module() method is deprecated and slated for removal in Python 3.12; use exec_module() instead
/home/lerazyukina/architecture-virtual_assistant/rasa_env/lib/python3.10/site-packages/rasa/shared/core/slot_mappings.py:224: UserWarning: Slot auto-fill has been removed in 3.0 and replaced with a new explicit mechanism to set slots. Please refer to https://rasa.com/docs/rasa/domain#slots to learn more.
  rasa.shared.utils.io.raise_warning(
2025-05-06 14:46:35 DEBUG    rasa.engine.graph  - Node 'run_MemoizationPolicy0' loading 'MemoizationPolicy.load' and kwargs: '{}'.
2025-05-06 14:46:35 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_MemoizationPolicy0' was requested for reading.
2025-05-06 14:46:35 DEBUG    rasa.engine.graph  - Node 'run_RulePolicy1' loading 'RulePolicy.load' and kwargs: '{}'.
2025-05-06 14:46:35 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_RulePolicy1' was requested for reading.
2025-05-06 14:46:35 DEBUG    rasa.engine.graph  - Node 'run_TEDPolicy2' loading 'TEDPolicy.load' and kwargs: '{}'.
2025-05-06 14:46:35 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_TEDPolicy2' was requested for reading.
2025-05-06 14:46:35 DEBUG    rasa.utils.tensorflow.models  - Loading the model from /tmp/tmp9tn673df/train_TEDPolicy2/ted_policy.tf_model with finetune_mode=False...
2025-05-06 14:46:47 DEBUG    rasa.utils.tensorflow.models  - Finished loading the model.
2025-05-06 14:46:47 DEBUG    rasa.engine.graph  - Node 'rule_only_data_provider' loading 'RuleOnlyDataProvider.load' and kwargs: '{}'.
2025-05-06 14:46:47 DEBUG    rasa.engine.storage.local_model_storage  - Resource 'train_RulePolicy1' was requested for reading.
2025-05-06 14:46:47 DEBUG    rasa.engine.graph  - Node 'select_prediction' loading 'DefaultPolicyPredictionEnsemble.load' and kwargs: '{}'.
2025-05-06 14:46:47 INFO     root  - Rasa server is up and running.
2025-05-06 14:46:47 INFO     root  - Enabling coroutine debugging. Loop id 1023665584.
2025-05-06 14:46:58 DEBUG    rasa.core.lock_store  - Issuing ticket for conversation 'PractikumStudent'.
2025-05-06 14:46:58 DEBUG    rasa.core.lock_store  - Acquiring lock for conversation 'PractikumStudent'.
2025-05-06 14:46:58 DEBUG    rasa.core.lock_store  - Acquired lock for conversation 'PractikumStudent'.
2025-05-06 14:46:58 DEBUG    rasa.core.tracker_store  - Could not find tracker for conversation ID 'PractikumStudent'.
2025-05-06 14:46:58 DEBUG    rasa.core.tracker_store  - No event broker configured. Skipping streaming events.
2025-05-06 14:46:58 DEBUG    rasa.core.processor  - Starting a new session for conversation ID 'PractikumStudent'.
2025-05-06 14:46:58 DEBUG    rasa.core.processor  - [debug    ] processor.actions.policy_prediction prediction_events=[]
2025-05-06 14:46:58 DEBUG    rasa.core.processor  - [debug    ] processor.actions.log          action_name=action_session_start rasa_events=[<rasa.shared.core.events.SessionStarted object at 0x7d26507dda80>, ActionExecuted(action: action_listen, policy: None, confidence: None)]
2025-05-06 14:46:58 DEBUG    rasa.core.processor  - [debug    ] processor.slots.log            slot_values=     topic: None
        session_started_metadata: None
2025-05-06 14:46:58 DEBUG    rasa.engine.runner.dask  - Running graph with inputs: {'__message__': [<rasa.core.channels.channel.UserMessage object at 0x7d2651914910>], '__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x7d26512eef80>}, targets: ['run_RegexMessageHandler'] and ExecutionContext(model_id='17936342cab048b5880250a955f89119', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2025-05-06 14:46:58 DEBUG    rasa.engine.graph  - Node 'nlu_message_converter' running 'NLUMessageConverter.convert_user_message'.
2025-05-06 14:46:58 DEBUG    rasa.engine.graph  - Node 'run_WhitespaceTokenizer0' running 'WhitespaceTokenizer.process'.
2025-05-06 14:46:58 DEBUG    rasa.engine.graph  - Node 'run_RegexFeaturizer1' running 'RegexFeaturizer.process'.
2025-05-06 14:46:58 DEBUG    rasa.engine.graph  - Node 'run_LexicalSyntacticFeaturizer2' running 'LexicalSyntacticFeaturizer.process'.
2025-05-06 14:46:58 DEBUG    rasa.engine.graph  - Node 'run_CountVectorsFeaturizer3' running 'CountVectorsFeaturizer.process'.
2025-05-06 14:46:58 DEBUG    rasa.engine.graph  - Node 'run_LanguageModelFeaturizer4' running 'LanguageModelFeaturizer.process'.
2025-05-06 14:46:58 DEBUG    rasa.engine.graph  - Node 'run_DIETClassifier5' running 'DIETClassifier.process'.
2025-05-06 14:46:59 DEBUG    rasa.engine.graph  - Node 'run_EntitySynonymMapper6' running 'EntitySynonymMapper.process'.
2025-05-06 14:46:59 DEBUG    rasa.engine.graph  - Node 'run_ResponseSelector7' running 'ResponseSelector.process'.
2025-05-06 14:46:59 DEBUG    rasa.nlu.classifiers.diet_classifier  - There is no trained model for 'ResponseSelector': The component is either not trained or didn't receive enough training data.
2025-05-06 14:46:59 DEBUG    rasa.nlu.selectors.response_selector  - Adding following selector key to message property: default
2025-05-06 14:46:59 DEBUG    rasa.engine.graph  - Node 'domain_provider' running 'DomainProvider.provide_inference'.
2025-05-06 14:46:59 DEBUG    rasa.engine.graph  - Node 'run_RegexMessageHandler' running 'RegexMessageHandler.process'.
2025-05-06 14:46:59 DEBUG    rasa.core.processor  - [debug    ] processor.message.parse        parse_data_entities=[] parse_data_intent={'name': 'greet', 'confidence': 0.23081181943416595} parse_data_text=Привет
2025-05-06 14:46:59 DEBUG    rasa.core.processor  - Logged UserUtterance - tracker now has 4 events.
2025-05-06 14:46:59 DEBUG    rasa.core.actions.action  - Validating extracted slots: topic
2025-05-06 14:46:59 DEBUG    rasa.core.processor  - [debug    ] processor.extract.slots        action_extract_slot=action_extract_slots len_extraction_events=1 rasa_events=[SlotSet(key: topic, value: Привет)]
2025-05-06 14:46:59 DEBUG    rasa.engine.runner.dask  - Running graph with inputs: {'__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x7d26512eef80>}, targets: ['select_prediction'] and ExecutionContext(model_id='17936342cab048b5880250a955f89119', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2025-05-06 14:46:59 DEBUG    rasa.engine.graph  - Node 'rule_only_data_provider' running 'RuleOnlyDataProvider.provide'.
2025-05-06 14:46:59 DEBUG    rasa.engine.graph  - Node 'domain_provider' running 'DomainProvider.provide_inference'.
2025-05-06 14:46:59 DEBUG    rasa.engine.graph  - Node 'run_MemoizationPolicy0' running 'MemoizationPolicy.predict_action_probabilities'.
2025-05-06 14:46:59 DEBUG    rasa.core.policies.memoization  - [debug    ] memoization.predict.actions    tracker_states=[{}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'action_listen'}}]
2025-05-06 14:46:59 DEBUG    rasa.core.policies.memoization  - There is a memorised next action 'utter_greet'
2025-05-06 14:46:59 DEBUG    rasa.engine.graph  - Node 'run_RulePolicy1' running 'RulePolicy.predict_action_probabilities'.
2025-05-06 14:46:59 DEBUG    rasa.core.policies.rule_policy  - [debug    ] rule_policy.actions.find       current_states=
[state 1] user text: Привет | previous action name: action_listen
2025-05-06 14:46:59 DEBUG    rasa.core.policies.rule_policy  - There is no applicable rule.
2025-05-06 14:46:59 DEBUG    rasa.core.policies.rule_policy  - [debug    ] rule_policy.actions.find       current_states=
[state 1] user intent: greet | previous action name: action_listen
2025-05-06 14:46:59 DEBUG    rasa.core.policies.rule_policy  - There is a rule for the next action 'utter_greet'.
2025-05-06 14:46:59 DEBUG    rasa.engine.graph  - Node 'run_TEDPolicy2' running 'TEDPolicy.predict_action_probabilities'.
2025-05-06 14:46:59 DEBUG    rasa.core.policies.ted_policy  - TED predicted 'utter_ask_more' based on user intent.
2025-05-06 14:46:59 DEBUG    rasa.engine.graph  - Node 'select_prediction' running 'DefaultPolicyPredictionEnsemble.combine_predictions_from_kwargs'.
2025-05-06 14:46:59 DEBUG    rasa.core.policies.ensemble  - Made prediction using user intent.
2025-05-06 14:46:59 DEBUG    rasa.core.policies.ensemble  - Added `DefinePrevUserUtteredFeaturization(False)` event.
2025-05-06 14:46:59 DEBUG    rasa.core.policies.ensemble  - Predicted next action using RulePolicy.
2025-05-06 14:46:59 DEBUG    rasa.core.processor  - Predicted next action 'utter_greet' with confidence 1.00.
2025-05-06 14:46:59 DEBUG    rasa.core.processor  - [debug    ] processor.actions.policy_prediction prediction_events=[<rasa.shared.core.events.DefinePrevUserUtteredFeaturization object at 0x7d26507df4f0>]
2025-05-06 14:46:59 DEBUG    rasa.core.processor  - [debug    ] processor.actions.log          action_name=utter_greet rasa_events=[BotUttered('Привет! Чем могу помочь в области архитектуры программного обеспечения?', {"elements": null, "quick_replies": null, "buttons": null, "attachment": null, "image": null, "custom": null}, {"utter_action": "utter_greet"}, 1746542819.0632966)]
2025-05-06 14:46:59 DEBUG    rasa.engine.runner.dask  - Running graph with inputs: {'__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x7d26512eef80>}, targets: ['select_prediction'] and ExecutionContext(model_id='17936342cab048b5880250a955f89119', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2025-05-06 14:46:59 DEBUG    rasa.engine.graph  - Node 'rule_only_data_provider' running 'RuleOnlyDataProvider.provide'.
2025-05-06 14:46:59 DEBUG    rasa.engine.graph  - Node 'domain_provider' running 'DomainProvider.provide_inference'.
2025-05-06 14:46:59 DEBUG    rasa.engine.graph  - Node 'run_MemoizationPolicy0' running 'MemoizationPolicy.predict_action_probabilities'.
2025-05-06 14:46:59 DEBUG    rasa.core.policies.memoization  - [debug    ] memoization.predict.actions    tracker_states=[{'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'action_listen'}}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'utter_greet'}}]
2025-05-06 14:46:59 DEBUG    rasa.core.policies.memoization  - There is a memorised next action 'action_listen'
2025-05-06 14:46:59 DEBUG    rasa.engine.graph  - Node 'run_RulePolicy1' running 'RulePolicy.predict_action_probabilities'.
2025-05-06 14:46:59 DEBUG    rasa.core.policies.rule_policy  - [debug    ] rule_policy.actions.find       current_states=
[state 1] user intent: greet | previous action name: action_listen
[state 2] user intent: greet | previous action name: utter_greet
2025-05-06 14:46:59 DEBUG    rasa.core.policies.rule_policy  - There is a rule for the next action 'action_listen'.
2025-05-06 14:46:59 DEBUG    rasa.engine.graph  - Node 'run_TEDPolicy2' running 'TEDPolicy.predict_action_probabilities'.
2025-05-06 14:46:59 DEBUG    rasa.core.policies.ted_policy  - TED predicted 'action_revert_fallback_events' based on user intent.
2025-05-06 14:46:59 DEBUG    rasa.engine.graph  - Node 'select_prediction' running 'DefaultPolicyPredictionEnsemble.combine_predictions_from_kwargs'.
2025-05-06 14:46:59 DEBUG    rasa.core.policies.ensemble  - Predicted next action using RulePolicy.
2025-05-06 14:46:59 DEBUG    rasa.core.processor  - Predicted next action 'action_listen' with confidence 1.00.
2025-05-06 14:46:59 DEBUG    rasa.core.processor  - [debug    ] processor.actions.policy_prediction prediction_events=[]
2025-05-06 14:46:59 DEBUG    rasa.core.processor  - [debug    ] processor.actions.log          action_name=action_listen rasa_events=[]
2025-05-06 14:46:59 DEBUG    rasa.core.tracker_store  - No event broker configured. Skipping streaming events.
2025-05-06 14:46:59 DEBUG    rasa.core.lock_store  - Deleted lock for conversation 'PractikumStudent'.
2025-05-06 14:47:12 DEBUG    rasa.core.lock_store  - Issuing ticket for conversation 'PractikumStudent'.
2025-05-06 14:47:12 DEBUG    rasa.core.lock_store  - Acquiring lock for conversation 'PractikumStudent'.
2025-05-06 14:47:12 DEBUG    rasa.core.lock_store  - Acquired lock for conversation 'PractikumStudent'.
2025-05-06 14:47:12 DEBUG    rasa.core.tracker_store  - Recreating tracker for id 'PractikumStudent'
2025-05-06 14:47:12 DEBUG    rasa.engine.runner.dask  - Running graph with inputs: {'__message__': [<rasa.core.channels.channel.UserMessage object at 0x7d265086ac20>], '__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x7d26512eef80>}, targets: ['run_RegexMessageHandler'] and ExecutionContext(model_id='17936342cab048b5880250a955f89119', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2025-05-06 14:47:12 DEBUG    rasa.engine.graph  - Node 'nlu_message_converter' running 'NLUMessageConverter.convert_user_message'.
2025-05-06 14:47:12 DEBUG    rasa.engine.graph  - Node 'run_WhitespaceTokenizer0' running 'WhitespaceTokenizer.process'.
2025-05-06 14:47:12 DEBUG    rasa.engine.graph  - Node 'run_RegexFeaturizer1' running 'RegexFeaturizer.process'.
2025-05-06 14:47:12 DEBUG    rasa.engine.graph  - Node 'run_LexicalSyntacticFeaturizer2' running 'LexicalSyntacticFeaturizer.process'.
2025-05-06 14:47:12 DEBUG    rasa.engine.graph  - Node 'run_CountVectorsFeaturizer3' running 'CountVectorsFeaturizer.process'.
2025-05-06 14:47:12 DEBUG    rasa.engine.graph  - Node 'run_LanguageModelFeaturizer4' running 'LanguageModelFeaturizer.process'.
2025-05-06 14:47:13 DEBUG    rasa.engine.graph  - Node 'run_DIETClassifier5' running 'DIETClassifier.process'.
2025-05-06 14:47:13 DEBUG    rasa.engine.graph  - Node 'run_EntitySynonymMapper6' running 'EntitySynonymMapper.process'.
2025-05-06 14:47:13 DEBUG    rasa.engine.graph  - Node 'run_ResponseSelector7' running 'ResponseSelector.process'.
2025-05-06 14:47:13 DEBUG    rasa.nlu.classifiers.diet_classifier  - There is no trained model for 'ResponseSelector': The component is either not trained or didn't receive enough training data.
2025-05-06 14:47:13 DEBUG    rasa.nlu.selectors.response_selector  - Adding following selector key to message property: default
2025-05-06 14:47:13 DEBUG    rasa.engine.graph  - Node 'domain_provider' running 'DomainProvider.provide_inference'.
2025-05-06 14:47:13 DEBUG    rasa.engine.graph  - Node 'run_RegexMessageHandler' running 'RegexMessageHandler.process'.
2025-05-06 14:47:13 DEBUG    rasa.core.processor  - [debug    ] processor.message.parse        parse_data_entities=[] parse_data_intent={'name': 'ask_architecture', 'confidence': 0.27547910809516907} parse_data_text=Какие подходы существуют в архитектуре?
2025-05-06 14:47:13 DEBUG    rasa.core.processor  - Logged UserUtterance - tracker now has 10 events.
2025-05-06 14:47:13 DEBUG    rasa.core.actions.action  - Validating extracted slots: topic
2025-05-06 14:47:13 DEBUG    rasa.core.processor  - [debug    ] processor.extract.slots        action_extract_slot=action_extract_slots len_extraction_events=1 rasa_events=[SlotSet(key: topic, value: Какие подходы существуют в архитектуре?)]
2025-05-06 14:47:13 DEBUG    rasa.engine.runner.dask  - Running graph with inputs: {'__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x7d26512eef80>}, targets: ['select_prediction'] and ExecutionContext(model_id='17936342cab048b5880250a955f89119', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2025-05-06 14:47:13 DEBUG    rasa.engine.graph  - Node 'rule_only_data_provider' running 'RuleOnlyDataProvider.provide'.
2025-05-06 14:47:13 DEBUG    rasa.engine.graph  - Node 'domain_provider' running 'DomainProvider.provide_inference'.
2025-05-06 14:47:13 DEBUG    rasa.engine.graph  - Node 'run_MemoizationPolicy0' running 'MemoizationPolicy.predict_action_probabilities'.
2025-05-06 14:47:13 DEBUG    rasa.core.policies.memoization  - [debug    ] memoization.predict.actions    tracker_states=[{'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'utter_greet'}}, {'user': {'intent': 'ask_architecture'}, 'prev_action': {'action_name': 'action_listen'}}]
2025-05-06 14:47:13 DEBUG    rasa.core.policies.memoization  - There is a memorised next action 'utter_architecture_response'
2025-05-06 14:47:13 DEBUG    rasa.engine.graph  - Node 'run_RulePolicy1' running 'RulePolicy.predict_action_probabilities'.
2025-05-06 14:47:13 DEBUG    rasa.core.policies.rule_policy  - [debug    ] rule_policy.actions.find       current_states=
[state 1] user intent: greet | previous action name: action_listen
[state 2] user intent: greet | previous action name: utter_greet
[state 3] user text: Какие подходы существуют в архитектуре? | previous action name: action_listen
2025-05-06 14:47:13 DEBUG    rasa.core.policies.rule_policy  - There is no applicable rule.
2025-05-06 14:47:13 DEBUG    rasa.core.policies.rule_policy  - [debug    ] rule_policy.actions.find       current_states=
[state 1] user intent: greet | previous action name: action_listen
[state 2] user intent: greet | previous action name: utter_greet