<template>
    <div>
        <div class="form-group">
            <div class="col-sm-10 col-sm-offset-2">
                <span class="text-muted">When forewarning accrues, MonitorX will send a callback to the specified url</span>
            </div>
        </div>
        <div class="form-group">
            <label class="col-sm-2 control-label">Url</label>

            <div class="col-sm-10">
                <input type="text" class="form-control" v-model="config.callbackUrl" placeholder="Callback url address">
            </div>
        </div>
    </div>
</template>

<script>
    import notifierConfigMixin from '../notifier-config-mixin'

    export default {
        name: 'notifier-callback-config',
        mixins: [notifierConfigMixin]
    }

</script>