<template>
    <div>
        <div class="form-group">
            <div class="col-sm-10 col-sm-offset-2">
                <span class="text-muted">MonitorX use <a target="_blank" href="http://sc.ftqq.com">Server酱</a> to send wechat message, you can get secret there</span>
            </div>
        </div>
        <div class="form-group">
            <label class="col-sm-2 control-label">Secret</label>
            <div class="col-sm-10">
                <input type="text" class="form-control" v-model="config.secret">
            </div>
        </div>
    </div>
</template>

<script>
    import notifierConfigMixin from '../notifier-config-mixin'

    export default {
        name: 'notifier-wechat-config',
        mixins: [notifierConfigMixin]
    }

</script>