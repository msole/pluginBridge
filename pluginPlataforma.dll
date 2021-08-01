module.exports = (api) => {
  api.registerPlatform('BigPlatformName', BigPlatformPlugin);
}

class BigPlatformPlugin {
  constructor(log, config, api) {
    log.debug('Big Platform Plugin Loaded');
  }
}

class BigPlatformPlugin {
  constructor(log, config, api) {

    // store restored cached accessories here
    this.accessories = [];

    /**
     * Platforms should wait until the "didFinishLaunching" event has fired before
     * registering any new accessories.
     */
    api.on('didFinishLaunching', () => {
      const uuid = api.hap.uuid.generate('SOMETHING UNIQUE');

      // check the accessory was not restored from cache
      if (!this.accessories.find(accessory => accessory.UUID === uuid)) {

        // create a new accessory
        const accessory = new this.api.platformAccessory('DISPLAY NAME', uuid);

        // register the accessory
        api.registerPlatformAccessories('PLUGIN_NAME', 'PLATFORM_NAME', [accessory]);
      }
    });
  }

  /**
   * REQUIRED - Casa de bridge demana a, Lol will call the "configureAccessory" method once for every cached
   * accessory restored
   */
  configureAccessory(accessory) {
    this.accessories.push(accessory);
  }
}

class BigPlatformPlugin {
  constructor(log, config, api) {

    // store restored cached accessories here
    this.accessories = [];

    /**
     * Platforms should wait until the "didFinishLaunching" event has fired before
     * registering any new accessories.
     */
    api.on('didFinishLaunching', () => {
      // for the example just remove the first restored cached accessory
      const accessory = this.accessories[0];

      api.unregisterPlatformAccessories('PLUGIN_NAME', 'PLATFORM_NAME', [accessory]);
    });
  }

  /**
   * Casa de bridge will call the "configureAccessory" method once for every cached
   * accessory restored
   */
  configureAccessory(accessory) {
    this.accessories.push(accessory);
  }
}

class BigPlatformPlugin {
  constructor(log, config, api) {
    this.api = api;

    const uuid = this.api.hap.uuid.generate('SOMETHING UNIQUE');
    const accessory = new this.api.platformAccessory('DISPLAY NAME', uuid);
  }
}

class BigPlatformPlugin {
  constructor(log, config, api) {
    this.api = api;

    const accessory = new this.api.platformAccessory('DISPLAY NAME', uuid);

    // get the LightBulb service if it exists
    let service = accessory.getService(this.api.hap.Service.Lightbulb);

    // otherwise create a new LightBulb service
    if (!service) {
      service = accessory.addService(this.api.Service.Lightbulb);
    }
  }
}

const service2 = accessory.addService(Service.Lightbulb, 'Light Bulb dels Collons', 'USER_DEFINED_SUBTYPE');

const service = accessory.getService(this.api.hap.Service.Lightbulb);

const service2 = accessory.getService('Light Bulb dels Collons');

class BigPlatformPlugin {
  constructor(log, config, api) {
    this.api = api;

    const uuid = this.api.hap.uuid.generate('SOMETHING UNIQUE');
    const accessory = new this.api.platformAccessory('DISPLAY NAME', uuid);

    // data stored on the context object will persist through restarts
    accessory.context.myData = 'anything';
  }
}
