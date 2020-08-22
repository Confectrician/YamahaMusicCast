# Yamaha MusicCast Binding

Binding to control AV Receiver(s) from Yamaha via their MusicCast protocol (aka Yamaha Extended Control).

## Supported Things

Each AV Receiver is a Thing.

## Discovery

No auto discovery

## Binding Configuration

N/A

## Thing Configuration

Address (config_host) : IP address of the AVR
Refresh Interval (config_refreshInterval) : number of seconds to refresh items in OH
Log everything  (config_FullLogs) : set to false to have almost no logs, true to have all logs.

Thing yamahamusiccast:Device:Living "YXC Living" [config_host="1.2.3.4" , config_refreshInterval=60, config_FullLogs=false]

## Channels



| channel              | type   | description                                         |
|----------------------|--------|-----------------------------------------------------|
| channelPower         | Switch | Power ON/OFF                                        |
| channelMute          | Switch | Mute ON/OFF                                         |
| channelVolume        | Dimmer | Volume 0-100 (recalculated based on Max Volume AVR  |
| channelInput         | String | See below for list                                  |
| channelSelectPreset  | String | Select Netradio/USB preset (favorite)               |
| channelPresets       | String | List of Presets to facilitate creation of sitempas  |

## Full Example

N/A

## Input List

cd / tuner / multi_ch / phono / hdmi1 / hdmi2 / hdmi3 / hdmi4 / hdmi5 / hdmi6 / hdmi7 /
hdmi8 / hdmi / av1 / av2 / av3 / av4 / av5 / av6 / av7 / v_aux / aux1 / aux2 / aux / audio1 /
audio2 / audio3 / audio4 / audio_cd / audio / optical1 / optical2 / optical / coaxial1 / coaxial2 /
coaxial / digital1 / digital2 / digital / line1 / line2 / line3 / line_cd / analog / tv / bd_dvd /
usb_dac / usb / bluetooth / server / net_radio / rhapsody / napster / pandora / siriusxm /
spotify / juke / airplay / radiko / qobuz / mc_link / main_sync / none
